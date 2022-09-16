<template>
  <div style="var(--va-secondary);">
    <va-sidebar hoverable textColor="dark" minimizedWidth="64px">
      <va-sidebar-item
        v-for="item in items"
        :key="item.title"
        :active="item.active"
      >
        <va-sidebar-item-content>
          <va-icon :name="item.icon" />
          <va-sidebar-item-title>
            {{ item.title }}
          </va-sidebar-item-title>
        </va-sidebar-item-content>
      </va-sidebar-item>
      <va-divider></va-divider>
    </va-sidebar>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { title: "Home", icon: "home" },
        { title: "Pesquisar", icon: "search" },
        { title: "Bolsistas", icon: "school" },
        { title: "Computadores", icon: "computer" },
        { title: "Projetos", icon: "folder" },
      ],
    };
  },
};
</script>
