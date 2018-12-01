# Overriding CSS with Emotion

You can use this module to override Bootstrap, Foundation, Semantic UI, ... and other styles with Emotion.

Get up and running with a single import.

```bash
npm install --save emotion
npm install --save emotion-css
```

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
