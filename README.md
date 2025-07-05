# 客户流失预测分析 ｜ Telco Customer Churn Prediction

本项目旨在通过机器学习模型预测电信行业客户流失行为，并提供可操作的商业策略建议，以帮助企业提升客户留存率。

This project uses machine learning models to predict customer churn in the telecom industry and offers actionable business insights to improve customer retention.

---

## 项目背景 | Project Background

客户流失会显著影响企业利润。通过对客户行为数据的建模，企业可以提前识别流失风险客户，进行个性化干预。

Customer churn significantly impacts business profitability. By modeling customer behavior data, companies can proactively identify at-risk users and take personalized actions.

---

## 数据集 | Dataset

- 来源：Kaggle - [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- 样本量：7,043 条客户数据
- 特征包括：合同类型、付款方式、月费、服务种类、是否流失等。

---

## 使用技术 | Technologies Used

- **Python**：数据处理与建模
- **Pandas / NumPy**：数据清洗与特征工程
- **Scikit-learn**：模型训练与评估
- **Matplotlib / Seaborn**：数据可视化
- **SMOTE / Class Weight**：处理类别不平衡问题
- **Colab**：项目开发平台

---

## 建模流程 | Modeling Workflow

1. 数据清洗与预处理（处理缺失值、编码、标准化等）
2. 探索性数据分析（EDA）
3. 特征工程（构造新变量、选择特征）
4. 多模型对比：
   - K-Nearest Neighbors (KNN)
   - Support Vector Machine (SVM)
   - Random Forest
   - Logistic Regression
5. 模型评估指标：
   - Accuracy
   - Precision / Recall / F1-Score
   - Confusion Matrix
   - ROC Curve & AUC

---

## 结果与分析 | Results & Insights

| Model | Accuracy | Recall (流失) | F1-Score (流失) |
|------|----------|----------------|-----------------|
| KNN  | 0.776     | 0.52           | 0.55            |
| SVM  | 0.808     | 0.50           | 0.58            |
| RF   | 0.809     | 0.50           | 0.58            |
| LR   | 0.814     | 0.50           | 0.58            |

> Random Forest 模型表现最稳定，AUC≈0.83，可作为最终部署模型。

The Random Forest model has the most stable performance with AUC ≈ 0.83 and can be used as the final deployment model.

---

## 💡 业务建议 | Business Recommendations

- 合同类型是流失最强预测因子 → 鼓励用户签订长期合同
  
  Contract type is the strongest predictor of churn → Encourage users to sign long-term contracts
- 电子账单用户更易流失 → 可通过纸质账单或个性化通知干预
  
  Electronic billing users are more likely to churn → can intervene with paper bills or personalized notifications
- 高月费客户流失率较高 → 可考虑提供会员奖励或定制优惠
  
  Higher churn rates for customers with high monthly fees → Consider offering membership rewards or customized offers


