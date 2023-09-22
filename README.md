# #JPA Delete 

# 

# #Validation 

## Empty ( no white space [""] )
    An empty value is a value that has no content. 
    Example : 
        - String  : ""
        - List    : []

## Blank ( white space [" "])
    A blank value is a value that is empty or contains only whitespace characters. 
    For example :
        - String   : “ “
        - List     : [ ]

## Notnull 
    A notnull value is a value that is not null.
    This means that the value must have a non-null value, but it can be empty or blank.
    Example  :
        - String  :  “abc”
        - List    : [1,2,3] mm

---
# JPA **`Relationship`**

## ManyToOne

    + Annotations:
      - @ManyToOne   
      - @JoinColumn 

## @ManyToOne properties Annotations

## @JoinColumn ManyToOne properties Annotations


```
    @ManyToOne
    @JoinColumn(name = "author_id") // Defines the foreign key column
    private Author author;
```

### Cascading:
    
    @ManyToOne(cascade = CascadeType.ALL)
    @JoinColumn(name = "author_id")
    private Author author;

### Fetch Type:
    
    @ManyToOne(fetch = FetchType.LAZY)
    @JoinColumn(name = "author_id")
    private Author author;

### Bidirectional Relationships:
    
    @Entity
    public class Author {

        @OneToMany(mappedBy = "author")
        private List<Book> books;
        
    }

# Security

    Password 
        + FrontEnd password:
        + FrontEnd password:

   + FrontEnd password:
     - b
     - e
   + BackEnd password:
     - bycript password 