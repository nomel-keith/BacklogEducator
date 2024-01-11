<template>
    <v-navigation-drawer
        expand-on-hover
        rail
      >
      <v-list>
        <v-list-item
          prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
          title="Keith Lemon"
          subtitle="keithlemon@gmail.com"
        ></v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-list density="compact" nav>
        <v-list-item :to="{ name: 'courses' }" prepend-icon="mdi-folder" title="My Courses" value="mycourses"></v-list-item>
        <v-list-item prepend-icon="mdi-account-multiple" title="Shared with me" value="shared"></v-list-item>
        <v-list-item prepend-icon="mdi-star" title="Starred" value="starred"></v-list-item>
      </v-list>      
    </v-navigation-drawer>
</template>