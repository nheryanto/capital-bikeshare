Introduction
-------------
Banyak kota di berbagai wilayah dunia sudah menerapkan sistem bike-sharing sebagai salah satu solusi masalah kepadatan lalu-lintas yaitu kemacetan, dan upaya untuk menurunkan emisi gas karbon yang berasal dari penggunaan kendaraan pribadi. Bike-sharing adalah sistem dimana sepeda disediakan oleh suatu instansi di berbagai titik lokasi dalam satu kota untuk dapat disewa oleh publik dalam jangka waktu tertentu, biasanya hitungan menit hingga jam dalam satu hari dan untuk jarak tempuh pendek. Melalui sistem bike-sharing, masyarakat didorong untuk mengurangi penggunaan kendaraan pribadi dengan beralih ke transportasi ramah lingkungan. Salah satu kota yang menerapkan sistem ini adalah Washington DC, ibukota Amerika Serikat. 

Capital Bikeshare merupakan sistem docked bike-sharing di Washington DC yang dimiliki oleh pemerintah setempat. Docked bike-sharing mempunyai sistem penyimpanan sepeda yang 'terkunci' di lokasi yang sudah ditentukan (disebut juga stasiun). Pengguna yang ingin menyewa sepeda dapat membuka kunci sepeda di stasiun keberangkatan dan memarkir sepeda di stasiun tujuan dengan mengunci kembali sepeda pada tempatnya. Mulai beroperasi pada September 2010 dengan meluncurkan 400 sepeda di 49 stasiun, Capital Bikeshare menjadi sistem bike-sharing terbesar di Amerika Serikat sampai tahun 2013. Motivator LLC merupakan kontraktor yang mengelola operasional Capital Bikeshare, mulai dari suplai ketersediaan sepeda hingga perawatan dan perbaikan sepeda.

Problem Statement
------------
Salah satu komponen penting yang menentukan kesuksesan bike-sharing adalah keseimbangan antara jumlah sepeda yang tersedia (supply) dengan jumlah pengguna sepeda (demand) pada setiap kondisi. Jika jumlah sepeda lebih sedikit dari kebutuhan, maka sistem dapat kehilangan pengguna atau pelanggan. Sebaliknya, jika jumlah sepeda lebih banyak dari jumlah pengguna, sistem menjadi tidak efisien dan dapat menambah biaya operasional hingga perawatan sepeda yang seharusnya bisa tidak perlu dikeluarkan.

Goals
------------
Dari permasalahan di atas, dengan mengetahui jumlah pengguna sepeda pada kondisi tertentu akan membantu stakeholder terkait yaitu penyedia sepeda (atau dalam konteks ini adalah kontraktor operasional Capital Bikeshare) dalam menentukan suplai sepeda. Jumlah pengguna sepeda ingin diprediksi seakurat mungkin atau mempunyai nilai error prediksi yang sekecil mungkin agar stakeholder dapat mengalokasikan jumlah sepeda tepat dengan kebutuhan sehingga tidak menghilangkan jumlah pengguna maupun menambahkan biaya operasional yang tidak perlu.

Analytic Approach
------------
Analisis data dilakukan untuk menemukan pola dan membangun model regresi yang dapat memprediksi jumlah pengguna sepeda berdasarkan kondisi suatu hari. Kita akan melihat apakah penggunaan sepeda dipengaruhi oleh cuaca dan musim, dan jika iya, bagaimana cuaca dan musim mempengaruhi penggunaan sepeda.

Metric Evaluation
------------
Metrik yang digunakan untuk mengevaluasi model adalah:
* Mean Absolute Error (MAE), atau rerata dari error absolut antara nilai prediksi dengan dengan nilai aktual
* Mean Absolute Percentage Error (MAPE), atau rerata dari persentase error antara nilai prediksi dengan dengan nilai aktual

Untuk MAE dan MAPE, semakin kecil nilainya maka semakin baik performa model karena nilai prediksi semakin mendekati nilai aktualnya. Akan tetapi, MAPE memiliki keterbatasan interpretasi ketika error prediksi lebih besar dari nilai aktualnya karena dengan begitu nilai persentasenya akan lebih besar dari 100%.

Project Organization
------------

    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── processed      <- The final, canonical data sets for analysis.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- The document will consist of a detailed analysis and visualization.
    │
    ├── notebooks          <- Jupyter notebooks. A naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    └── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
                              generated with `pip freeze > requirements.txt`

--------
