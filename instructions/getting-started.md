# Fabric OneLake as Central Storage

### Overall Estimated Duration: 1 Hour 30 minutes

## Overview

In this lab, you will explore a range of modern data onboarding techniques within the Microsoft Fabric platform. Using the iconic Gapminder scatter chart as inspiration—a dynamic visualization that illustrates the relationship between life expectancy and GDP per capita across countries—you will ingest, integrate, and model data from four distinct sources: Azure SQL Database, Amazon S3, Snowflake, and virtual files. Once the data is unified within a Fabric Lakehouse, you will use Power BI to recreate the Gapminder-style animated bubble chart, where each country is represented as a bubble positioned by its income and life expectancy, sized by population, and animated across time to visualize global development trends.

## Objective

Learn how to build and orchestrate AI-driven agents for intelligent customer service using Azure AI Services. By the end of this lab, you will be able to:

- **Fabric OneLake as Central Storage:** Learn to onboard, integrate, and visualize diverse datasets using Microsoft Fabric, creating impactful insights with Power BI and a unified data architecture.

## Pre-requisites

- **Familiarity with Azure**: Basic knowledge of Azure services and the Azure portal for managing cloud resources.

- **Basic Knowledge of Fabric**: Understanding of Microsoft Fabric concepts and workflows.

## Architecture

This architecture centralizes data storage and analytics using Microsoft Fabric OneLake as the unified storage layer, enabling seamless data integration, mirroring, and visualization across platforms. Data flows originate from sources like Data Studio and SQL Server databases, which are ingested into a centralized Lakehouse environment. External data, such as files stored in AWS S3 Buckets, are also incorporated into the Lakehouse. To maintain consistency and real-time access, data from Snowflake is mirrored into the Lakehouse. This unified data is then stored in OneLake and made available for dynamic reporting and insights through Power BI visualizations. The architecture supports scalable, cloud-native analytics while ensuring interoperability across hybrid storage solutions and analytics platforms.

## Architecture Diagram

![](../media/arch.png)

## Explanation of Components

- **Data Studio:** Acts as the data entry or reporting interface, initiating data workflows that are processed through SQL Server systems.

- **SQL Server & Database:** Serves as a foundational data source and processing layer, facilitating data ingestion into the Lakehouse for centralized analytics.

- **AWS S3 Bucket:** Provides external object storage, enabling additional data sources to be integrated into the Lakehouse environment.

- **Lakehouse:** Functions as the unified analytics engine that consolidates ingested data and mirrored sources, enabling structured and unstructured data analysis.

- **Snowflake:** A cloud-based data platform whose datasets are mirrored into the Lakehouse, ensuring consistency and access across analytics workflows.

- **OneLake Storage:** Acts as the centralized storage solution within the Microsoft Fabric ecosystem, standardizing data access across tools and services.

- **Power BI:** Empowers users with rich, interactive dashboards and visual analytics derived from the data stored in OneLake.

## Getting Started with Lab

Welcome to Fabric OneLake as Central Storage Lab ! , We've prepared a seamless environment for you to explore and learn. Let's begin by making the most of this experience.

>**Note:** If a PowerShell window appears once the environment is active, please don't close it. Minimize it instead of closing it and proceed with the tasks.

### Accessing Your Lab Environment

Once you're ready to dive in, your virtual machine and Lab guide will be right at your fingertips within your web browser.

![](./media/gs-1n.png)

### Exploring Your Lab Resources

To get a better understanding of your Lab resources and credentials, navigate to the Environment tab.

![](./media/gs-2n.png)

### Utilizing the Split Window Feature

For convenience, you can open the Lab guide in a separate window by selecting the Split Window button from the Top right corner

![](./media/gs-3n.png)

### Managing Your Virtual Machine

Feel free to start, stop, or restart your virtual machine as needed from the Resources tab. Your experience is in your hands!

![](./media/gs-4n.png)

## Let's Get Started with Azure Portal

1. In the JumpVM, click on **Azure portal** shortcut of Microsoft Edge browser which is created on desktop.

   ![](./media/gs-5n.png)

1. On the **Sign into Microsoft Azure** tab, you will see the login screen. Enter the provided email or username, and click **Next** to proceed.

   - Email/Username: <inject key="AzureAdUserEmail"></inject>

     ![](./media/gs-6n.png)

1. Now, enter the following password and click on **Sign in**.

   - Password: <inject key="AzureAdUserPassword"></inject>

     ![](./media/gs-7n.png)

     >**Note:** If you see the Action Required dialog box, then select Ask Later option.
     
1. If you see the pop-up **Stay Signed in?**, click No.

1. If you see the pop-up **You have free Azure Advisor recommendations!**, close the window to continue the Lab.

1. If a **Welcome to Microsoft Azure** popup window appears, click **Cancel** to skip the tour.

## Support Contact

The CloudLabs support team is available 24/7, 365 days a year, via email and live chat to ensure seamless assistance at any time. We offer dedicated support channels tailored specifically for both learners and instructors, ensuring that all your needs are promptly and efficiently addressed.Learner Support Contacts:

- **Email Support:** cloudlabs-support@spektrasystems.com
- **Live Chat Support:** https://cloudlabs.ai/labs-support

Now, click on Next from the lower right corner to move on to the next page.

## Happy Learning!!