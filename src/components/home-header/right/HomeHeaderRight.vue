<template>
  <div id="home-header-right">
    <header-carousel :slides="slides" />
  </div>
</template>

<script>
import HeaderCarousel from "@/components/home-header/right/header-carousel/HeaderCarousel";
export default {
name: "HomeHeaderRight",
  components: {HeaderCarousel},
  data: () => ({
    slides: [
      {
        img: 'https://images.unsplash.com/photo-1453738773917-9c3eff1db985?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=750&q=80'
      },
      {
        img: 'https://images.unsplash.com/photo-1517245386807-bb43f82c33c4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80'
      },
      {
        img: 'https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60'
      },
      {
        img: 'https://images.unsplash.com/photo-1517607908060-9a66da662869?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60'
      },
      {
        img: 'https://images.unsplash.com/photo-1515187029135-18ee286d815b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60'
      },
      {
        img: 'https://images.unsplash.com/photo-1486312338219-ce68d2c6f44d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60'
      },
      {
        img: 'https://images.unsplash.com/photo-1483699862560-f524a8c11c6c?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1658&q=80'
      },
      {
        img: 'https://images.unsplash.com/photo-1476003992331-1f0ab9241f34?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1268&q=80'
      }
    ]
  })
}
</script>

<style scoped>

</style>
