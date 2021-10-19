# DBテーブルカラム詳細一覧

### 購入テーブル (d_purchase)
|和名|属性名|型|PK|NN|FK|
|:---|:---|:---|:---|:---|:---:|
|オーダーID|order_id|bigint(20)|○|○||
|顧客コード|customer_code|varchar(50)||○||
|購入日|purchase_date|date||○||
|総額|total_price|int(11)||○||

### PCパーツ詳細テーブル(d_purchase_detail)
|和名|属性名|型|PK|NN|FK|
|:---|:---|:---|:---|:---|:---:|
|オーダー詳細ID|detail_id|bigint(20)|○|○||
|オーダーID|order_id|bigint(20)|○|○|○|
|os商品コード|os_code|int(11)||○||
|os価格|os_price|int(11)||○||
|CPU商品コード|cpu_code|int(11)||○||
|CPU在庫|cpu_stock|int(11)||○||
|CPU価格|cpu_price|int(11)||○||
|CPU数量|cpu_num|int(20)||○||
|メモリ商品コード|memory_code|int(11)||○||
|メモリ在庫|memory_stock|int(11)||○||
|メモリ価格|memory_price|int(11)||○||
|メモリ数量|memory_num|int(20)||○||
|GPU商品コード|gpu_code|int(11)||○||
|GPU在庫|gpu_stock|int(11)||○||
|GPU価格|gpu_price|int(11)||○||
|GPU数量|gpu_num|int(20)||○||
|SSD商品コード|ssd_code|int(11)||○||
|SSD在庫|ssd_stock|int(11)||○||
|SSD価格|ssd_price|int(11)||○||
|SSD数量|ssd_num|int(20)||○||
|HDD商品コード|hdd_code|int(11)||○||
|HDD在庫|hdd_stock|int(11)||○||
|HDD価格|hdd_price|int(11)||○||
|HDD数量|hdd_num|int(20)||○||

### 顧客マスター(m_customers)
|和名|属性名|型|PK|NN|FK|
|:---|:---|:---|:---|:---|:---:|
|顧客コード|customer_code|varchar(50)|○|○||
|パスワード|pass|varchar(50)|○|○||
|氏名|name|varchar(100)||○||
|電話番号|tel|varchar(20)||○||
|メール|mail|varchar(100)||○||
|削除フラグ|del_flag|int(11)||||
|登録日|reg_date|date||○||

### カテゴリマスタ　(m_category)
|和名|属性名|型|PK|NN|FK|
|:---|:---|:---|:---|:---|:---:|
|カテゴリID|category_id|int(11)|○|○||
|氏名|name|varchar(20)||○||
|登録日|reg_date|date||○||

### 商品マスタ (m_item)
|和名|属性名|型|PK|NN|FK|
|:---|:---|:---|:---|:---|:---:|
|商品コード|item_id|int(11)|〇|〇||
|価格|price|int(11)||〇||
|PCタイプ|pc_cate|int(11)||〇||
|OS|os_id|int(11)||〇||
|CPU|cpu_id|int(11)||〇||
|メモリー|memory_id|int(11)||〇||
|GPU|gup_id|int(11)||〇||
|SSD|ssd_id|int(11)||〇||
|HDD|hdd_id|int(11)||〇||

