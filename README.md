# docs

# **Table of Contents**

- [Cypress](#cypress)
  - [Usefull Tool](#cypress_tool)
  - [Run Cypress](#cypress_run)
  - [Methods](#cypress_commands)

---

# Cypress
<a name="cypress"></a>

## Tools
<a name="cypress_tool"></a>

- [Testing Playground](https://chrome.google.com/webstore/detail/testing-playground/hejbmebodbijjdhflfknehhcgaklhano)

## Run cypress
<a name="cypress_run"></a>

```
node_modules/.bin/cypress open
```
## Commands
<a name="cypress_commands"></a>

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

Get element by id or by css class that define the element
```
cy.get('#email').type('fake@email.com').should('have.value', 'fake@email.com')
```
or
```
cy.get('.action-email').type('fake@email.com').should('have.value', 'fake@email.com')
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

```
...should('have.value', 'some value')
```

```
...should('include', 'something')
```

```
...should('exist')
```



