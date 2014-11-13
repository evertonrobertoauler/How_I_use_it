# MongoDB

## Commands

show all databases

    show dbs

use database

    use dbname
    
drop selected database

    db.dropDatabase()
    
show all collections

    show collections
    
drop a collection

    db.collectionname.drop()

insert a document

    db.collectionname.insert({fieldname: 'test name'})

update field on documents

    db.collectionname.update(
      {name: 'test name'}, 
      {$set: {fieldname: 'new value'}}, 
      {upsert: true, multi: true}
    )

delete document

    db.collectionname.remove({fieldname: 'test name'})
