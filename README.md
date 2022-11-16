# pyspark
Test performance of pyspark on MNIST dataset in Google Collab

Important note - argmax needs to be used on predicted labels by fitted_pipeline.transform(test_df), because it returns predictions as lists of label probablilities, when only indice of softmax value is supported:
https://stackoverflow.com/questions/59951319/how-to-get-the-index-of-the-highest-value-in-a-list-per-row-in-a-spark-dataframe