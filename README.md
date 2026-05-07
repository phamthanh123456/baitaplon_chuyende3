--- DỰ ĐOÁN GIÁ NHÀ ---

Môi trường cài đặt, sử dụng
- Visual Studio Code
- Jupyter Notebook 

Tổng quan bài toán và dữ liệu
- Bài toán: Dự đoán giá nhà từ các thông tin cơ bản của một căn hộ (vị trí xây, diện tích,số phòng, tiện nghi,...) 
- Dữ liệu sử dụng: Giá các căn hộ được bán tại Ames, Iowa từ 2006 đến 2010. Dữ liệu dùng 1460 mẫu cho tập train train.

Link dataset: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data
Dataset name : house-prices-advanced-regression-techniques


Tổng dữ liệu: 1460
- 1460 dòng
- 80 cột
Train(70%): 1022 mẫu
Validation(30%): 438 mẫu

Có 1460 mẫu dữ liệu huấn luyện và 1460 mẫu dữ liệu kiểm tra. Tổng số thuộc tính là 81, trong đó 36 thuộc tính định lượng, 43 thuộc tính định tính cộng với ID và SalePrice.
Quantitative: 1stFlrSF, 2ndFlrSF, 3SsnPorch, BedroomAbvGr, BsmtFinSF1, BsmtFinSF2, BsmtFullBath, BsmtHalfBath, BsmtUnfSF, EnclosedPorch, Fireplaces, FullBath, GarageArea, GarageCars, GarageYrBlt, GrLivArea, HalfBath, KitchenAbvGr, LotArea, LotFrontage, LowQualFinSF, MSSubClass, MasVnrArea, MiscVal, MoSold, OpenPorchSF, OverallCond, OverallQual, PoolArea, ScreenPorch, TotRmsAbvGrd, TotalBsmtSF, WoodDeckSF, YearBuilt, YearRemodAdd, YrSold

Qualitative: Alley, BldgType, BsmtCond, BsmtExposure, BsmtFinType1, BsmtFinType2, BsmtQual, CentralAir, Condition1, Condition2, Electrical, ExterCond, ExterQual, Exterior1st, Exterior2nd, Fence, FireplaceQu, Foundation, Functional, GarageCond, GarageFinish, GarageQual, GarageType, Heating, HeatingQC, HouseStyle, KitchenQual, LandContour, LandSlope, LotConfig, LotShape, MSZoning, MasVnrType, MiscFeature, Neighborhood, PavedDrive, PoolQC, RoofMatl, RoofStyle, SaleCondition, SaleType, Street, Utilities


Tổ chức github
Folders
- Experiment/ : chứa notebook thực hiện các thực nghiệm.
Files
- main.ipynb: notebook chính dùng để báo cáo.
- data_description.txt : mô tả đầy đủ của từng cột.
- test.csv : bộ dữ liệu thử nghiệm.
- train.csv : tập dữ liệu huấn luyện.
- gbr_final.csv : tệp chứa kết quả dự báo cuối cùng từ mô hình Gradient Boosting Regressor (GBR).
- lasso_final.csv : tệp lưu trữ các dự đoán được tạo ra bởi mô hình Lasso Regression.
- ridge_final.csv : tệp lưu trữ kết quả từ mô hình Ridge Regression.
- xgb_final.csv : tệp lưu trữ kết quả đầu ra của mô hình XGBoost (Extreme Gradient Boosting).
- sample_submission.csv : tệp mẫu định dạng cấu hình cột và hàng.
- test_result.csv : tệp chứa kết quả dự báo tổng hợp hoặc cuối cùng trên bộ dữ liệu kiểm tra (test set) sau khi bạn đã lựa chọn hoặc kết hợp các mô hình tốt nhất.



