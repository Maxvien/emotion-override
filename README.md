# Overriding CSS styles with Emotion

You can use **emotion** to override Bootstrap, Foundation, Semantic UI, ... CSS styles without `!important`.

### Install

```bash
npm install --save emotion
npm install --save emotion-css
```

### Usage

```javascript
import css from 'emotion-css';

const app = document.getElementById('root');

// String Style
const stringStyle = css`
  font-size: 14px;
  border: none;
`;

// Object Style
const objectStyle = css({
  color: 'red',
  background: 'yellow'
});


app.classList.add(stringStyle);
app.classList.add(objectStyle);
```
