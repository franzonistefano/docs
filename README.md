# docs

# **Table of Contents**

- [Cypress](#cypress)

---

# Cypress

## Run cypress

```
node_modules/.bin/cypress open
```
## Commands
<a name="cypress"></a>

- [visit](#visit)
- [get](#get)
- [type](#type)
- [contains](#contains)
- [url](#url)
- [should](#should)

<a name="visit"></a>
### Visit

Visit specific url

```
cy.visit('http://localhost:3000/')
```

<a name="get"></a>
### Get

Get element by id
```
cy.get('#email').type('fake@email.com').should('have.value', 'fake@email.com')
```

<a name="type"></a>
### Type

type text on getted element
```
cy.get('#email').type('fake@email.com').should('have.value', 'fake@email.com')
```

<a name="contains"></a>
### Contains

Get element which contains specific text
```
cy.contains('Enter').click()
```

<a name="url"></a>
### Url

Check if url contains specific word inside the path
```
cy.url().should('include', 'homepage')
```

<a name="should"></a>
### Should



