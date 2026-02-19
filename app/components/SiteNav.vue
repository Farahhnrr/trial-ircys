<template>
  <header class="top">
    <div class="brand">
      <img class="brand-logo" src="/img/logo.png" alt="International Research Competition logo" />
    </div>

    <nav class="top-nav" aria-label="Primary">
      <ul class="nav-list">
        <li
          v-for="item in siteNav"
          :key="item.to"
          class="nav-item"
          :class="{
            'has-children': item.children?.length,
            'is-active': isActive(item),
            'is-open': openItem === item.to
          }"
        >
          <NuxtLink :to="item.to" class="nav-link">
            {{ item.label }}
          </NuxtLink>
          <button
            v-if="item.children?.length"
            class="nav-toggle"
            type="button"
            :aria-expanded="openItem === item.to"
            :aria-label="`Toggle ${item.label} submenu`"
            @click="toggleItem(item.to)"
          >
            <span aria-hidden="true">▾</span>
          </button>
          <div v-if="item.children?.length" class="nav-submenu" role="menu">
            <NuxtLink
              v-for="child in item.children"
              :key="child.to"
              :to="child.to"
              class="nav-sublink"
              role="menuitem"
            >
              {{ child.label }}
            </NuxtLink>
          </div>
        </li>
      </ul>
    </nav>

    <button class="nav-cta" type="button">Register</button>
  </header>
</template>

<script setup lang="ts">
import { siteNav, type NavItem } from "../data/siteNav";

const route = useRoute();
const openItem = ref<string | null>(null);

const isActive = (item: NavItem) => {
  if (route.path === item.to) {
    return true;
  }

  if (item.children?.some((child) => route.path === child.to)) {
    return true;
  }

  return route.path.startsWith(`${item.to}/`);
};

const toggleItem = (key: string) => {
  openItem.value = openItem.value === key ? null : key;
};
</script>

<style scoped>
.top {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  position: relative;
  z-index: 9999;
  gap: 2rem;
  flex-wrap: wrap;
}

.brand {
  display: flex;
  align-items: center;
  min-width: 140px;
}

.brand-logo {
  width: 140px;
  height: 140px;
  object-fit: contain;
}

.top-nav {
  flex: 1 1 520px;
  max-width: 100%;
  position: relative;
  z-index: 9999;
}

.nav-list {
  list-style: none;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 2rem 3rem;
  padding: 0;
  margin: 0;
}

.nav-item {
  position: relative;
  display: flex;
  align-items: center;
  gap: 0.35rem;
  z-index: 9999;
  padding-bottom: 0.6rem;
}

.nav-link {
  color: #1f1b15;
  text-decoration: none;
  font-size: 0.85rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  border-bottom: 1px solid transparent;
  padding-bottom: 0.2rem;
  transition: border-color 160ms ease;
}

.nav-item.is-active .nav-link,
.nav-link:hover,
.nav-link:focus {
  border-bottom-color: #1f1b15;
}

.nav-submenu {
  position: absolute;
  top: 100%;
  left: 0;
  min-width: 220px;
  display: grid;
  gap: 0.5rem;
  background: rgba(255, 255, 255, 0.96);
  padding: 0.9rem 1rem;
  border-radius: 16px;
  box-shadow: 0 16px 30px rgba(60, 47, 32, 0.16);
  opacity: 0;
  transform: translateY(6px);
  pointer-events: none;
  transition: opacity 160ms ease, transform 160ms ease;
  z-index: 10000;
}

.nav-item.has-children:hover .nav-submenu,
.nav-item.has-children:focus-within .nav-submenu,
.nav-item.is-open .nav-submenu {
  opacity: 1;
  transform: translateY(0);
  pointer-events: auto;
}

.nav-sublink {
  color: #2b231a;
  text-decoration: none;
  font-size: 0.86rem;
  padding: 0.35rem 0.2rem;
  border-radius: 8px;
  transition: background-color 160ms ease;
}

.nav-sublink:hover,
.nav-sublink:focus {
  background: rgba(163, 123, 75, 0.12);
}

.nav-toggle {
  border: none;
  background: transparent;
  color: #1f1b15;
  font-size: 0.9rem;
  cursor: pointer;
  padding: 0.2rem 0.35rem;
  line-height: 1;
}

.nav-toggle:focus-visible {
  outline: 2px solid rgba(31, 27, 21, 0.35);
  outline-offset: 2px;
  border-radius: 6px;
}

.nav-cta {
  border: 1px solid #a37b4b;
  background: #ffffff;
  color: #a37b4b;
  padding: 0.6rem 1.6rem;
  border-radius: 999px;
  font-size: 0.85rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  transition: background-color 160ms ease, transform 160ms ease;
}

.nav-cta:hover,
.nav-cta:focus {
  background: #f1ede6;
  transform: translateY(-1px);
}

@media (max-width: 900px) {
  .top {
    flex-direction: column;
    align-items: flex-start;
  }

  .nav-list {
    justify-content: flex-start;
    gap: 1.4rem 2rem;
  }

  .nav-submenu {
    position: static;
    opacity: 1;
    transform: none;
    pointer-events: auto;
    box-shadow: none;
    padding: 0.6rem 0 0;
    background: transparent;
  }

  .nav-item {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.4rem;
  }

  .nav-cta {
    align-self: flex-start;
  }
}
</style>
