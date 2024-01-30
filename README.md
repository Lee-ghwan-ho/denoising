
---
## grayscale image denoising-




---
## 24.01.30
rank 1	KBNe t29.54		
KBNet: Kernel Basis Network for Image Restoration
# 연구과제에 필요한 image_denoising 모델을 찾다가, grayscale image denoising sota 모델 이용
![image](https://github.com/Lee-ghwan-ho/denoising/assets/114568122/86588dbf-b3a1-463e-a046-7fe28544888f)
- 1.학습된 pretrained_model을 다운 받음(파일위치:https://mycuhk-my.sharepoint.com/personal/1155135732_link_cuhk_edu_hk/_layouts/15/onedrive.aspx?id=%2Fpersonal%2F1155135732%5Flink%5Fcuhk%5Fedu%5Fhk%2FDocuments%2Fshare%2FKBNet&ga=1)
- 2.gau_gray_15.pth,gau_gray_25.pth,gau_gray_50.pth 중 우리에게 잘 맞는 것은 gau_gray_25.pth로 판단 
- 3. denoising 한장당 6분정도 (gpu 3090 24gb)
- 4. denoising 한 이미지를 teed로 boundary detection ->결과: 제일 좋은 성능 보여줌 
---
