##  Model Relationships

####ONE-TO-ONE
```
DS.belongsTo
```

####ONE-TO-MANY & MANY-TO-MANY
```
DS.hasMany
```


NOTE:
 sometimes you may have multiple belongsTo/hasManys for the same type. 
 You can specify which property on the related model is the inverse using DS.hasMany's inverse option: