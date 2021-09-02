<template>
  <v-container>
    <h3 class="display-2 text-center mb-4">Our Pricing</h3>
    <p class="body-1 text-center mb-4"></p>

    <div class="pricing-wrap">
      <v-row justify="center">
        <v-col md="9">
          <v-row align="end">
            <v-col
              v-for="(tier, index) in tiers"
              :key="index"
              md="4"
              sm="tier.title === 'enterpris' ? 12 : 4"
              class="px-5"
            >
              <pricing-card
                class="pc"
                :img="tier.img"
                :title="tier.title"
                :description="tier.description"
                :price="tier.price"
                :button-text="tier.buttonText"
                :button-variant="tier.buttonVariant"
              />
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<style scoped lang="scss">
@import './pricing-style';
</style>

<script>
import PricingCard from '../Cards/PricingCard'

export default {
  components: {
    PricingCard,
  },
  data() {
    return {
      tiers: [
        {
          title: 'Basic Plan',
          img: 'https://png.pngtree.com/png-clipart/20190515/original/pngtree-bule-border-png-image_3551748.jpg',

          description: [
            '5 GB bandwidth',
            'Highest Speed',
            '1 GB Storage',
            'Unlimited Website',
            '24x7 Greate Support',
          ],
          price: '549',
          buttonText: 'SELECT',
          buttonVariant: 'outlined',
        },
        {
          title: 'Advanced Plan',
          img: 'https://genial-react.envytheme.com/images/icon2.png',

          description: [
            '5 GB bandwidth',
            'Highest Speed',
            '1 GB Storage',
            'Unlimited Website',
            '24x7 Greate Support',
          ],
          price: '749',
          buttonText: 'SELECT',
          buttonVariant: 'outlined',
        },
        {
          title: 'Expert Plan',
          img: 'https://genial-react.envytheme.com/images/icon3.png',

          description: [
            '5 GB bandwidth',
            'Highest Speed',
            '1 GB Storage',
            'Unlimited Website',
            '24x7 Greate Support',
          ],
          price: '949',
          buttonText: 'SELECT',
          buttonVariant: 'outlined',
        },
      ],
    }
  },
}
</script>
