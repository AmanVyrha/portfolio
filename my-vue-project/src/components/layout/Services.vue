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
    heading: "Time Series Forecasting for Stock Prices",
    description:
      "Built a predictive model using LSTM networks to forecast stock prices based on historical market data. This project showcases my skills in time series analysis and deep learning.",
    anothertext: "View the code and analysis on GitHub",
    label: "Check it out!",
    link: "https://github.com/AmanVyrha/stock-price-forecasting",
  },
  {
    heading: "Customer Segmentation Using K-means Clustering",
    description:
      "Applied unsupervised learning to segment customers based on purchasing behavior. This analysis helps in targeted marketing strategies and customer relationship management.",
    anothertext: "Explore the clustering analysis on GitHub",
    label: "View Project",
    link: "https://github.com/AmanVyrha/customer-segmentation",
  },
  {
    heading: "Risk Assessment in Insurance Industry",
    description:
      "Developed a risk assessment model for insurance underwriting using statistical methods and Monte Carlo simulations. This project demonstrates my ability to assess financial and operational risks.",
    anothertext: "See the project details on GitHub",
    label: "Learn More",
    link: "https://github.com/AmanVyrha/insurance-risk-assessment",
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
