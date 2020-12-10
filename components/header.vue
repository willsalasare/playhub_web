<template>
  <nav class="flex justify-between p-5">
    <div>
      <nuxt-link class="text-2xl" to="/"
        ><img width="150px" src="@/assets/logo.png"
      /></nuxt-link>
    </div>
    <ul class="flex">
      <li v-for="(item, i) in items" :key="i" class="p-2">
        <a :href="item.to">
          <img :src="item.icon" width="20px" />
        </a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          name: "Facebook",
          to: "https://www.facebook.com/playhubplus",
          icon: "https://www.facebook.com/images/fb_icon_325x325.png",
        },
        {
          name: "Instagram",
          to: "https://instagram.com/playhubplus",
          icon:
            "https://www.instagram.com/static/images/ico/favicon-192.png/68d99ba29cc8.png",
        },
        {
          name: "Telegram",
          to: "https://t.me/playhubplus",
          icon: "https://telegram.org/favicon.ico?4",
        },
      ],
    };
  },
};
</script>
