---
title: "Create measures from templates"
description: "Define measures using templates for common use cases."
ms.date: 03/25/2022

ms.subservice: audience-insights
ms.topic: conceptual
author: v-wendysmith
ms.author: wameng
ms.reviewer: v-wendysmith
manager: shellyha
searchScope: 
  - ci-measure-template
  - customerInsights
---

# Use a template to build a measure

You can use predefined templates of commonly used [measures](measures.md) to create them. Detailed descriptions of the templates and a guided experience help you with efficient measure creation. Templates build on mapped data from the *Unified Activity* entity. So make sure you have configured [customer activities](activities.md) before you create a measure from a template.

To create custom measures, see [Use measure builder to create measures from scratch](measure-builder.md).

# [Individual consumers (B-to-C)](#tab/b2c)

Available measure templates: 
- Average transaction value (ATV)
- Total transaction value
- Average daily revenue
- Average yearly revenue
- Transaction count
- Loyalty points earned
- Loyalty points redeemed
- Loyalty points balance
- Active customer lifespan
- Loyalty membership duration
- Time since last purchase

## Build a new measure using a template

1. Go to **Measures**.

1. Select **New** and select **Choose a template**.

   :::image type="content" source="media/measure-use-template.png" alt-text="Screenshot of the dropdown menu when creating a new measure with highlight on template.":::

1. Find the template that fits your need and select **Choose template**.

1. Review the required data and select **Get started** if you have all the data in place.

1. Select **Edit details** next to Measure name. Provide a name for the measure. Optionally, add [tags](work-with-tags-columns.md#manage-tags) to the measure.

   :::image type="content" source="media/measures_edit_details.png" alt-text="Edit details dialog box.":::

1. Select **Done**.

1. In the **Set time period** section, define the time frame of the data to use. Choose if you want the new measure to cover the entire dataset by selecting **All time**, or if you want the measure to focus on a **Specific time period**.

   :::image type="content" source="media/measure-set-time-period.png" alt-text="Screenshot showing the time period section when configuring a measure from a template.":::

1. In the next section, select **Add data** to choose the activities and map the corresponding data from your *Unified Activity* entity.

    1. Step 1 of 2: Under **Activity type**, choose the type of the entity you want to use. For **Activities**, select the entities you want to map.
    1. Step 2 of 2: Choose the attribute from the *Unified Activity* entity for the component required by the formula. For example, for Average transaction value, it's the attribute representing the Transaction value. For **Activity timestamp**, choose the attribute from the Unified Activity entity that represents the date and time of the activity.
   
1. Once the data mapping is successful, you can see the status as **Complete** and the name of the mapped activities and attributes.

1. You can now select **Run** to calculate the results of the measure. To refine it later, select **Save draft**.

# [Business accounts (B-to-B)](#tab/b2b)

This feature is only available for measures created in environments with individual customers as primary target audience.

---
