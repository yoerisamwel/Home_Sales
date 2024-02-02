# Home_Sales

As part of the GWU bootcamp, we delved into the practical applications of the PySpark library, harnessing its robust capabilities for real-world data analysis. Our exploration was centered around a Home Sales dataset conveniently housed in an AWS S3 bucket. Initially, we set the stage by configuring the Spark environment and establishing a SparkSession, the cornerstone for our subsequent data operations.

We embarked on our analytical journey by ingesting the dataset into a PySpark DataFrame, followed by the creation of a temporary view named home_sales. This setup paved the way for a series of insightful SQL queries, enabling us to unravel various facets of the dataset. We calculated average home prices based on specific criteria such as the number of bedrooms, bathrooms, and the year the home was built. Particularly, we honed in on homes with distinctive features like multiple floors and a minimum square footage, showcasing the nuanced analytical capabilities of PySpark.

Aiming to enhance performance, we leveraged PySpark's caching mechanism, which significantly expedited our data retrieval operations. This optimization was evident when we revisited certain queries, observing a marked reduction in runtime. Furthermore, we explored data partitioning by writing our DataFrame to a Parquet file, partitioned based on the date_built field. This strategy not only streamlined our storage but also optimized our data querying process.

Our analysis culminated with a meticulous examination of homes priced at or above $350,000, focusing on their "view" ratings. We meticulously measured and compared the runtime of this operation on both cached and partitioned data, gaining valuable insights into performance optimization techniques.

Finally, we demonstrated responsible resource management by uncaching our DataFrame, ensuring an efficient allocation and release of computational resources. This comprehensive exploration not only bolstered our understanding of PySpark's capabilities but also highlighted its profound implications in real-world data analysis scenarios, particularly within the realm of Home Sales data.
