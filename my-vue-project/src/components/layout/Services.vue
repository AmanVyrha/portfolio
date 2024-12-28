<script setup>
import SeeMoreVue from "../common/TheOtherCard.vue";
import ServicesBox from "../common/ServicesBox.vue";
import TheOtherCard from "../common/TheOtherCard.vue";



const cards = [
  {
    heading: "Predictive Analytics Model",
    description:
      "Developed a machine learning model to predict sales trends using historical data. The model uses regression techniques to forecast future sales, helping businesses make data-driven decisions.",
    anothertext: "See the full project on GitHub",
    label: "Explore Now",
    link: "https://github.com/AmanVyrha/sales-prediction-model",
  },
  {
    heading: "Data Cleaning and ETL Pipeline",
    description:
      "Built a robust data cleaning and transformation pipeline to handle large, messy datasets. This project highlights my expertise in automating the ETL process and preparing data for analysis.",
    anothertext: "Check out the pipeline implementation on GitHub",
    label: "Explore Now",
    link: "https://github.com/AmanVyrha/data-cleaning-etl-pipeline",
  },
];



</script>

<template>
  <div class="flex flex-col w-full gap-5">
    <p class="text-sm text-button_text pl-2.5">Services</p>
    <div class="flex flex-col gap-3">
      <ServicesBox
        v-for="(card, index) in cards"
        :key="index"
        :heading="card.heading"
        :description="card.description"
        :anothertext="card.anothertext"
        :label="card.label"
        :link="card.link"
      />
      <TheOtherCard />
    </div>
  </div>
</template>
