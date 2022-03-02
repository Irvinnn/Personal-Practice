kurang lebih gambaran EDA:

- import data (ya iyalah)
- liat2 dulu datanya
	- .head() (ngintip dikit datanya)
	- .shape() (self describe lah ya)
	- .describe() (statistical infonya gitu mean, std)
	- .info() (nama kolom dan jumlahnya, bisa buat cek null)
	- .nunique() (jumlah data unik)

- cleaning2 dikit la
	- .drop() (menjatuhkan sesama oh bukan ya)
	- .value_counts() (hitung jumlahnya bisa buat perbadingan gitu)
	- categorical to numerical (either ordinal or one hot)
		- pd.get_dummies()  (ganti ke one hot)
		- pake else if kalo ordinal 
	- split data-data yang masih bisa dipecah lagi
		df[''].split('.')[0]

- cari korelasi antar variabel 
	- .loc[df['']==1] (cek data spesifik)
	- .groupby('').mean() (dicek berdasarkan tipe sebuah kolom)
	- pd.crosstab() (ngeliat jumlah berdasarkan kolom spesifik)
	- .corr() and sns.heatmap() (plot correlation heatmap)
	- sns.pairplot() (lebih detil dari yang di atas)
	- sns.relplot() (kayak pairplot tapi individu)
	- sns.boxplot() (enak lah buat plotting data)

- urus missing value
	- kalo ga penting di drop aja (kalo data lo berjibun la)
	- kalo penting bisa pake mean dari sebuah kolom yang paling berkorelasi (kayak umur sama gelar)
	- pake scatter and hue bisa bantu cari korelasi

