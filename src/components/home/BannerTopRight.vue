<template>
  <div class="col-sm-6 nopadding banner-right">
    <div class="aspect-ratio aspect-ratio--4to3">
      <BannerPicture :file="'top-right.jpg'"/>
    </div>

    <div class="banner-text">
      <h4 class="banner-title">{{ $t('title') }}</h4>
      <p class="banner-paragraph">{{ $t('subtitle') }}</p>
      <router-link :to="{ name: 'products', params: { categorySlug: 'women-bags' } }"
                   class="btn banner-btn">
        {{ $t('linkLabel') }}
      </router-link>
    </div>
  </div>
</template>

<script>
import BannerPicture from './BannerPicture.vue';

export default {
  components: { BannerPicture },
};
</script>

<i18n>
en:
  title: "Summer Essentials"
  subtitle: "Make the great day happen"
  linkLabel: "Shop collection"
de:
  title: "Sommer Essentials"
  subtitle: "Die wichtigsten Stücke des Sommer Trends"
  linkLabel: "Jetzt bestellen"
</i18n>
