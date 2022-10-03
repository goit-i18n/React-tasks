# Lesson №1

## Creating components (no styling)

### Task №1

Break [layout](<https://www.figma.com/file/mfsNEI7Nv5i5fkdseWbFn7/Lesson-(Copy)?node-id=8701%3A11194>) into components

**For example**

```jsx
<Sidebar>
<Menu>
<MenuItem>
<Main>
<Paper>
<Card>
<TutorsList>
<Tutor>
<CitiesList>
<City>
<DepartmentsList>
<Department>
```

### Task №2

Create a menu.js file where there will be an array for drawing the menu

```jsx
export const menuConfig = [
  {
    name: "University",
  },

  {
    name: "Faculties",
  },
];
```

Draw menu in sidebar using `menuConfig` and show work with `props` and `key`

![Menu](/images/sidebar.png)

### Task №3

Create a `<Paper>` component - a component with a white background and padding that uses `props.children` and renders whatever markup is passed to it

![Paper](/images/paper.png)

### Task №4

Render the card and description component using ` <Paper>` and show how to import images into the component

Card

![Card](/images/Card.png)

Description

![description](/images/description.png)

### Task №5

Draw collections of teachers, cities, faculties using this json

```json
{
  "name": "MIT",
  "description": "Experience, a concentration of knowledge and the ability to avoid most recruiting mistakes. We know what most local and foreign companies want and we can give it to you. And we are constantly improving our programming courses, adding something new there. You can see the success stories of our alumni for yourself to see the effectiveness of our teaching methodology. Yes, we will start with the basics and the most basic information. We know that most people come to us with zero knowledge.",
  "tutors": [
    {
      "firstName": "John",
      "lastName": "Smith",
      "patronymic": "Александровна",
      "phone": "+38(097) 448 73 11",
      "email": "johnsmith@goit.global,
      "city": "New York",
      "options": "Group creation"
    },
    {
      "firstName": "Елена",
      "lastName": "Иванова",
      "patronymic": "Александровна",
      "phone": "+38(093) 443 43 51",
      "email": "ivanova.mail@gmail.com",
      "city": "Berlin",
      "options": "Group creation, editing teacher profiles"
    }
  ],
  "cities": ["Kyiv", "Londpn", "Berlin"],
  "department": [
    { "name": "Faculty of computer science and computer engineering" },
    { "name": "Faculty of Artificial Intelligence" },
    { "name": "Faculty of analytics" }
  ]
}
```

![collection](/images/collection.png)

### Task №6

Create a generic button component that will have 3 props `text`, `icon` and `onClick` (in the future)

![button](/images/button.png)

### Task №7

Make prog descriptions inside all components using `propTypes`
