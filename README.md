# AI Product Description Generator  
### (CampusCart – AIML Feature Module)

This repository contains the **AIML feature module** developed as part
of the **CampusCart** campus marketplace project. The module generates
professional, sell-worthy product descriptions using a product image and
optional user-provided text.


# Purpose

In campus marketplaces, product listings often have incomplete or
informal descriptions. This module improves listing quality by
automatically generating **clear, buyer-oriented descriptions** using
image understanding and NLP techniques.

# Workflow

The system follows a sequential pipeline to process data:

1.  **Product Image Input**

2.  **Image Captioning:** Powered by Vision Models.

3.  **Image Insight Extraction:** Hybrid approach using Rules and
    Zero-Shot NLP.

4.  **User Description Analysis:** Optional refinement based on seller
    input.

5.  **Selling-Oriented Generation:** Synthesis of final text.

6.  **Final Product Description:** Output intended for user display.

# Key Features

-   **Image-based understanding:** Automated detection of product
    categories.

-   **Hybrid insight extraction:** Specialized for campus items like
    coding books and reference guides.

-   **User description enhancement:** Merges raw user notes with
    AI-generated professional tone.

-   **Framework-independent design:** Modular architecture for easy
    backend integration.

# Entry Point

The primary function for this module is:

> `describe_product_from_image(image_path, user_description=None)`

  **Parameter**        **Requirement**   **Description**
  -------------------- ----------------- ------------------------------------------------------------
  `image_path`         Mandatory         Path to the product image file.
  `user_description`   Optional          Additional text provided by the user to refine the output.

  : Module Input Specifications

# Technologies Used

## Computer Vision

-   **BLIP Image Captioning:** `Salesforce/blip-image-captioning-base`

## Natural Language Processing

-   **Zero-Shot Classification:** `facebook/bart-large-mnli`

## Design Approach

-   **Hybrid AI:** Utilizing a combination of Rules and ML for accuracy
    and explainability.

# Scope

This repository focuses solely on the **AIML logic**. It does *not*
include frontend code, backend APIs, authentication, or database
integration.
