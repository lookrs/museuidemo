<template>
  <div class="InfoList">
    <mu-list textline="two-line">
      <mu-divider></mu-divider>
      <mu-list-item avatar :ripple="false" button>
        <mu-list-item-content>
          <mu-list-item-title>Ali Connors</mu-list-item-title>
          <mu-list-item-sub-title style="color: rgba(0, 0, 0, .87)">Brunch this weekend?</mu-list-item-sub-title>
          <mu-list-item-sub-title>I'll be in your neighborhood doing errands this weekend. Do you want to hang out?</mu-list-item-sub-title>
        </mu-list-item-content>
        <mu-list-item-action>
          <mu-list-item-after-text>15 min</mu-list-item-after-text>
          <mu-checkbox
            color="yellow700"
            v-model="selects"
            value="value1"
            uncheck-icon="star_border"
            checked-icon="star"
          ></mu-checkbox>
        </mu-list-item-action>
      </mu-list-item>
      <mu-divider></mu-divider>
      <mu-list-item avatar :ripple="false" button>
        <mu-list-item-content>
          <mu-list-item-title>me, Scrott, Jennifer</mu-list-item-title>
          <mu-list-item-sub-title style="color: rgba(0, 0, 0, .87)">Summer BBQ</mu-list-item-sub-title>
          <mu-list-item-sub-title>Wish I could come, but I'm out of town this weekend.</mu-list-item-sub-title>
        </mu-list-item-content>
        <mu-list-item-action>
          <mu-list-item-after-text>2 hr</mu-list-item-after-text>
          <mu-checkbox
            color="yellow700"
            v-model="selects"
            value="value2"
            uncheck-icon="star_border"
            checked-icon="star"
          ></mu-checkbox>
        </mu-list-item-action>
      </mu-list-item>
      <mu-divider></mu-divider>
      <mu-list-item avatar :ripple="false" button>
        <mu-list-item-content>
          <mu-list-item-title>Sandra Adams</mu-list-item-title>
          <mu-list-item-sub-title style="color: rgba(0, 0, 0, .87)">Oui oui</mu-list-item-sub-title>
          <mu-list-item-sub-title>Do you have Paris recommendations? Have you ever been?</mu-list-item-sub-title>
        </mu-list-item-content>
        <mu-list-item-action>
          <mu-list-item-after-text>6 hr</mu-list-item-after-text>
          <mu-checkbox
            color="yellow700"
            v-model="selects"
            value="value3"
            uncheck-icon="star_border"
            checked-icon="star"
          ></mu-checkbox>
        </mu-list-item-action>
      </mu-list-item>
      <mu-divider></mu-divider>
      <mu-list-item avatar :ripple="false" button>
        <mu-list-item-content>
          <mu-list-item-title>Sandra Adams</mu-list-item-title>
          <mu-list-item-sub-title style="color: rgba(0, 0, 0, .87)">Oui oui</mu-list-item-sub-title>
          <mu-list-item-sub-title>Do you have Paris recommendations? Have you ever been?</mu-list-item-sub-title>
        </mu-list-item-content>
        <mu-list-item-action>
          <mu-list-item-after-text>6 hr</mu-list-item-after-text>
          <mu-checkbox
            color="yellow700"
            v-model="selects"
            value="value3"
            uncheck-icon="star_border"
            checked-icon="star"
          ></mu-checkbox>
        </mu-list-item-action>
      </mu-list-item>
      <mu-divider></mu-divider>
      <mu-list-item avatar :ripple="false" button>
        <mu-list-item-content>
          <mu-list-item-title>Sandra Adams</mu-list-item-title>
          <mu-list-item-sub-title style="color: rgba(0, 0, 0, .87)">Oui oui</mu-list-item-sub-title>
          <mu-list-item-sub-title>Do you have Paris recommendations? Have you ever been?</mu-list-item-sub-title>
        </mu-list-item-content>
        <mu-list-item-action>
          <mu-list-item-after-text>6 hr</mu-list-item-after-text>
          <mu-checkbox
            color="yellow700"
            v-model="selects"
            value="value3"
            uncheck-icon="star_border"
            checked-icon="star"
          ></mu-checkbox>
        </mu-list-item-action>
      </mu-list-item>
      <mu-divider></mu-divider>
      <mu-list-item avatar :ripple="false" button>
        <mu-list-item-content>
          <mu-list-item-title>Sandra Adams</mu-list-item-title>
          <mu-list-item-sub-title style="color: rgba(0, 0, 0, .87)">Oui oui</mu-list-item-sub-title>
          <mu-list-item-sub-title>Do you have Paris recommendations? Have you ever been?</mu-list-item-sub-title>
        </mu-list-item-content>
        <mu-list-item-action>
          <mu-list-item-after-text>6 hr</mu-list-item-after-text>
          <mu-checkbox
            color="yellow700"
            v-model="selects"
            value="value3"
            uncheck-icon="star_border"
            checked-icon="star"
          ></mu-checkbox>
        </mu-list-item-action>
      </mu-list-item>
    </mu-list>
  </div>
</template>

<script>
export default {
  name: "InfoList",
  data() {
    return {
      selects: [],
    };
  },
};
</script>

<style scoped>
.InfoList {
  overflow: auto;
  max-height: 380px;
}
</style>