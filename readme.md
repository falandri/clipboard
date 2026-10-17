# How to customize tailwindcss

## Optional vscode plugins

- tailwindcss intellisense

## Cusomize font

Required actions: import font family in the firs line of src/styles.css file

```
@import url("https://fonts.googleapis.com/css2?family=Bai+Jamjuree:wght@400;600&display=swap");
```

```
module.exports = {
  content: ['./*.html'],
    theme: {
      extend: {
        fontFamily: {
          sans: ['Bai Jamjuree', 'sans-serif'],
        },
      },
    },
  plugins: [],
}
```

## Customize colors

```
module.exports = {
  content: ['./*.html'],
    theme: {
      extend: {
        colors: {
          strongCyan: 'hsl(171, 66%, 44%)',
          lightBlue: 'hsl(233, 100%, 69%)',
          darkGrayishBlue: 'hsl(210, 10%, 33%)',
          grayishBlue: 'hsl(201, 11%, 66%)',
        },
      },
    },
  plugins: [],
}
```

## Customize breakpoints

```
module.exports = {
  content: ['./*.html'],
    theme: {
      screens: {
        sm: '480px',
        md: '768px',
        lg: '976px',
        xl: '1440px',
      },
      extend: {},
    },
  plugins: [],
}
```
