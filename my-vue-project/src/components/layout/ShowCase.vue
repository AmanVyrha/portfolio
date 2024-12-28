<script setup>
import ShowCaseCard from "../common/ShowCaseCard.vue";
import { swift_summarizer, astra, alleviate, eventsync } from "../../assets";



const cards = [
  {
    title: "Predictive Analytics Model",
    description: "Sales Forecasting Using Machine Learning",
    imgSrc: predictive_analytics_image,  // Replace with actual image source
    imgAlt: "Sales Forecasting",
    link: "https://github.com/AmanVyrha/sales-prediction-model",  // Replace with your GitHub repo link
  },
  {
    title: "Time Series Forecasting for Stock Prices",
    description: "Predicting Stock Market Trends Using LSTM Networks",
    imgSrc: time_series_forecasting_image,  // Replace with actual image source
    imgAlt: "Stock Price Prediction",
    link: "https://github.com/AmanVyrha/stock-price-forecasting",  // Replace with your GitHub repo link
  },
  {
    title: "Customer Segmentation Using K-means Clustering",
    description: "Segmenting Customers Based on Purchasing Behavior",
    imgSrc: customer_segmentation_image,  // Replace with actual image source
    imgAlt: "Customer Segmentation",
    link: "https://github.com/AmanVyrha/customer-segmentation",  // Replace with your GitHub repo link
  },
  {
    title: "Risk Assessment in Insurance",
    description: "Monte Carlo Simulations for Risk Evaluation",
    imgSrc: risk_assessment_image,  // Replace with actual image source
    imgAlt: "Risk Assessment",
    link: "https://github.com/AmanVyrha/insurance-risk-assessment",  // Replace with your GitHub repo link
  },
  {
    title: "Data Cleaning and ETL Pipeline",
    description: "Automated Data Transformation Pipeline for Large Datasets",
    imgSrc: data_cleaning_image,  // Replace with actual image source
    imgAlt: "Data Cleaning Pipeline",
    link: "https://github.com/AmanVyrha/data-cleaning-etl-pipeline",  // Replace with your GitHub repo link
  },
];
</script>

<template>
  <div class="flex flex-col w-full gap-5">
    <p class="text-sm text-button_text pl-2.5" >Showcase</p>
    <div class="flex flex-col gap-3">
      <ShowCaseCard
        v-for="(card, index) in cards"
        :key="index"
        :title="card.title"
        :description="card.description"
        :imgSrc="card.imgSrc"
        :imgAlt="card.imgAlt"
        :link="card.link"
      />
    </div>
  </div>
</template>
