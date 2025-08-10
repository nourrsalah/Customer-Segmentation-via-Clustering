##  Overview
Applies unsupervised machine learning to segment customers based on demographics and spending behavior.  
Compares multiple clustering algorithms and evaluates their performance.  
Approach is adaptable for **grouping schools, communities, or beneficiaries** in development programs.

---

## Tech Stack
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Algorithms:** KMeans, Hierarchical Clustering, Gaussian Mixture Model (GMM), BIRCH  
- **Dimensionality Reduction:** PCA for visualization

---

## Steps
1. Data cleaning and encoding categorical variables  
2. Feature scaling with StandardScaler  
3. PCA transformation to 2D space  
4. Clustering using 4 different algorithms  
5. Model evaluation with:
   - **Silhouette Score** (higher is better)  
   - **Davies-Bouldin Index** (lower is better)  

---

## Results
| Algorithm       | Silhouette Score | Davies-Bouldin Index |
|-----------------|------------------|----------------------|
| KMeans          | 0.272            | 1.181                |
| Hierarchical    | 0.287            | 1.220                |
| GMM             | 0.222            | 1.211                |
| BIRCH           | 0.291            | 1.194                |

- **Best performer:** BIRCH (highest silhouette score)
- Clear spending-based customer groups identified

