 * REPOSITORY: inferential-stats-calc
 * FILE: README.md
 * VERSION: 1.0.0
 * DESCRIPTION: Documentation for the Statistical Inference Solver Web App.
 */

# Statistical Inference Solver

A professional, interactive web application designed to automate and visualize complex statistical calculations. This tool focuses on **Hypothesis Testing (t-Student)** and **Confidence Intervals for Proportions**, specifically tailored to handle scenarios like pharmaceutical reaction time studies and financial credit compliance.

## 🚀 Key Features

*   **Student's t-Test Module**:
    *   Calculates the **t-statistic** for small samples ($n < 30$) when the population standard deviation is unknown.
    *   Supports **One-tailed** (Left/Right) and **Two-tailed** tests.
    *   Features a dynamic **Conclusion Engine** that automatically interprets results against critical values.
*   **Confidence Interval Module**:
    *   Estimates the true **population proportion** using sample data.
    *   Provides standard confidence levels: **90%, 95%, and 99%**.
    *   Calculates the **Margin of Error** and displays the final interval clearly.
*   **Interactive Visualizations**:
    *   Uses **Chart.js** to render probability density functions (PDF).
    *   Highlights **Rejection Regions** and specific data points for better conceptual understanding.

## 🛠️ Technical Stack

*   **Frontend**: HTML5, CSS3 (Modern, tab-based UI).
*   **Engine**: Vanilla JavaScript (ES6+) for mathematical logic and DOM manipulation.
*   **Charts**: Chart.js (via CDN) for real-time distribution plotting.

## 📦 Implementation & Deployment

1.  **File Structure**: Save the code as `index.html`.
2.  **Hosting**: Upload to a GitHub repository named `inferential-stats-calc`.
3.  **GitHub Pages**:
    *   Go to **Settings > Pages**.
    *   Select the `main` branch and click **Save**.
    *   The app will be live at `https://[your-username].github.io/inferential-stats-calc/`.

## 📝 Technical Logic

*   **t-Distribution**: The app approximates the distribution using the Gamma function to plot the curve accurately for different degrees of freedom ($df = n - 1$).
*   **Critical Values**: Integrated lookup tables provide precise values for $\alpha = 0.10, 0.05, 0.01$ based on standard statistical tables.
*   **Proportion Logic**: Uses the Normal distribution approximation for large sample sizes ($n=400$) as seen in fintech scenarios.
