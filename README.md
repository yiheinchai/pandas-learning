# Learning Points
## Slicers
- Key Concepts
  - iloc and loc are used to slice the dataframe
  - iloc means to slice using the index
  - loc means to slice using specific values
- Syntax
  - iloc[<row_filter>, <column_filter>]
  - loc[<row_filter>, <column_filter>]
- Filter syntax (iloc)
  - <start>:<end>
  - For example, iloc[2:4,3:10] will filter rows from index 2-3, and columns from index 3-9
- Filter syntax (loc)
  - <row_filter> Pass in a series containing data of the rows you want to keep
  - For example, df.loc[df['<column_name>'].isin(['value1', 'value2']), <column_filter>]
  - Moreover, instead of passing in a series, you can pass the data of the rows directly with an array
  - For example, df.loc[['row1_column_2_value']] <-- this will return all column of row 1
  - <column_filter> Pass in an array or series of the columns you want to keep
  - For example, df.loc[<row_filter>, ['column1', 'column2']
