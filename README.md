bq extract --destination_format CSV --compression GZIP --noprint_header deribit.history 'gs://deribit_bk/history_1_*.csv'


bq load --source_format=CSV deribit.x1 'gs://deribit_bk/history_1_*.csv'