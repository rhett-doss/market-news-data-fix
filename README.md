# Stock Market News Data Filler

This project is a demonstration of my approach to processing and filling missing stock market news data. The system is built around two main components: `news_pipeline` and `source_fix`.

## Overview

### 1. Source Fix

#### Purpose

The `source_fix` component processes news data based on timestamps. Its primary role is to sort and categorize news data according to unique dates in the Eastern Time (ET) zone.

#### Key Features

- **File Cleaning:** Initial steps involve cleaning up old output files to ensure a fresh start during each run.
- **Timezone Conversion:** One of the main features is the conversion of timestamps from UTC to the US/Eastern timezone.
- **File Segregation:** After processing, the data is output into separate CSV files, each dedicated to a unique date.

### 2. News Pipeline

#### Purpose

The `news_pipeline` component is a more intricate processor of news data. It is responsible for transforming and enhancing the structure and content of the input data.

#### Key Features

- **Data Preprocessing:** This includes tasks like adjusting symbols in the news data and ensuring timestamps are in the correct format.
- **Symbol Management:** A significant portion of the logic is dedicated to managing the expiry of symbols based on predefined time intervals.
- **Structured Outputs:** The processed news data is handled daily, with outputs structured around specific symbol lists.
- **Post-Processing:** After generating the primary outputs, specific patterns in the output files are replaced to match desired formats.

## Note

This README is intended to provide a brief overview of the project's design and capabilities. The project is not meant for direct replication or use by others but rather as a showcase of my work in this domain.
