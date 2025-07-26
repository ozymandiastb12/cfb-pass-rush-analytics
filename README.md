# CFB Pass Rush Performance Analysis

## Overview

Analysis of college football pass rushers to identify top performers and relationships between pass rush grades and win rates using PFF 2024 season data. Creates professional visualizations with automatic labeling of elite players.

## 🔗 Key Findings

- Strong positive correlation (r ≈ 0.7) between pass rush grade and win rate
- Edge defenders average higher win rates than defensive interior players
- Elite threshold: 85+ grade OR (80+ grade & 15+ win rate)
- Only 12% of players achieve elite performance classification
- High-volume players (400+ snaps) maintain consistent efficiency

## Data Source

PFF College Football pass rush data with 300+ snap minimum threshold

## Tools Used

- R with tidyverse, ggplot2, ggrepel, viridis packages
- Custom CFB-themed visualization styling
- Performance tier classification system
- Automated top performer identification

## Methodology

- **Elite Performers**: Grade ≥ 85 OR (Grade ≥ 80 & Win Rate ≥ 15%) OR (Grade ≥ 75 & Win Rate ≥ 18%)
- **Position Groups**: ED (Edge Defender), DI (Defensive Interior)
- **Minimum Thresholds**: 300 pass rush snaps
- **Performance Tiers**: Elite (80+), Good (70-79), Average (60-69), Below Average (<60)

## Usage

```r
# Install required packages
install.packages(c("tidyverse", "ggrepel", "viridis"))

# Run analysis
source("cfb_pass_rush_analytics.R")
# Select CSV file when prompted
