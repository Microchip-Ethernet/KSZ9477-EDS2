# KSZ9477-EDS2
KSZ9477 EDS2 Platform binaries

For building DSA image for KSZ9477S EDS2 + SAMA7D65 Curiosity, please refer to https://microchip.my.site.com/s/article/How-to-build-DSA-image-for-SAMA7D65-EVB-KSZ9477-EDS2

For building non-DSA image for KSZ9477S EDS2 + SAMA7D65 Curiosity，please refer to following:  
git clone https://github.com/Microchip-Ethernet/EVB-LAN9646.git  
cd EVB-LAN9646/  
cd buildroot-at91-linux4microchip-2023.10/  
echo $PATH  
export PATH=/opt/mscc/sam-ba_v3.8:$PATH  
echo $PATH  
make BR2_EXTERNAL=../ung_apps_external sama7d65_curiosity_mmc_defconfig  
make  
cd output/images/  

KSZ9477S EDS2 Daughter Card User Guide:  
https://ww1.microchip.com/downloads/aemDocuments/documents/UNG/ProductDocuments/UserGuides/KSZ9477S-EDS2-Daughter-Card-User-Guide-DS50003928.pdf  

AN3474 KSZ9477 High-Availability Seamless Redundancy Application Note:  
https://www.microchip.com/en-us/application-notes/an3474  
