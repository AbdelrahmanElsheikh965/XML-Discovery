### Using: cd-catalog.xml

• Write a suitable **XPath** Expression for following use cases:

1. Select all the CD's titles with price more than 10$   
```
/catalog/cd[price>10]/title
```

2. Select all the CDs that came before 1990  
```
/catalog/cd[year<1990]
```

3. Select the titles and prices of all the CDs from "UK"  
```
/catalog/cd[country="UK"]/title | /catalog/cd[country="UK"]/price  
```
**Another Solution:**   
```
//cd[country="UK"]/title | //cd[country="UK"]/price
```

4. Select the artists names in the CDs that came before "someOne" 's CD  
```
/catalog/cd[artist = 'someOne']/preceding::cd/artist
```

5. Select the titles of all the CDs after the "anotherOne" CD  
```
/catalog/cd[artist = 'anotherOne']/following-sibling::cd/title
```
