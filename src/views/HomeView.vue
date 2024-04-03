<template>
  <v-container>
    <v-row v-for="item in notices" :key="item.year">
      <v-col cols="12">
        <v-card tile hover>
          <v-card-title>{{ item.year }} 年度</v-card-title>
          <v-card-subtitle>
            期間: {{ item.from }} - {{ item.to }}
          </v-card-subtitle>
          <v-divider class="mt-3"/>
          <v-card-text v-if="item.balance_sheet !== ''">
            {{ item.balance_sheet }}
          </v-card-text>
          <v-card-text v-else>
            未掲載
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang="ts" setup>

import {ref} from "vue";

const notices = ref([
  {
    "year": "2024",
    "from": "2024-04-01",
    "to": "2025-03-31",
    "balance_sheet": ""
  }
])
</script>
