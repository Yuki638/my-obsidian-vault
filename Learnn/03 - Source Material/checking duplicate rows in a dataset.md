lets see if you got any duplicate rows in your [[dataset]]

lets check with the [[jupyter notebook]] snippet 
![[Pasted image 20240922152840.png]]
 
# what if you found a duplicate value actually

no worries we just need to use `drop` function just use

```python
stock_df.drop_duplicates(inplace= True)
```
