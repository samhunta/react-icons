
<img src="https://rawgit.com/gorangajic/react-icons/master/react-icons.svg" width="60" alt="React Icons">
## [React Icons](http://gorangajic.github.io/react-icons/index.html)

Include popular icons in you react project easly with ```react-icons```. It uses ES6 imports so you can only include icons that your project is using.

### installation
    npm install react-icons --save

### usage
```javascript
import FaBeer from 'react-icons/fa/FaBeer';

class Question extends React.Component {
    render() {
        return <h3> Lets go for a <FaBeer />? </h3>
    }
}
````

you can include icon directly from ```react-icons``` using ```import FaBeer from 'react-icons'``` but you should wait to webpack 2 [implement](https://twitter.com/dan_abramov/status/656970508005736448) dead code elimination based on es6 imports

### Icons

Currenlty supported icons are
* Material Design Icons by Google https://www.google.com/design/icons/ (licence: [CC-BY 4.0](https://github.com/google/material-design-icons/blob/master/LICENSE))
* Font Awesome by Dave Gandy - http://fontawesome.io (licence: [SIL OFL 1.1](http://scripts.sil.org/OFL))
* Typicons by Stephen Hutchings - http://typicons.com (licence: [CC BY-SA](http://creativecommons.org/licenses/by-sa/3.0/))

you can add more icons by creating pull request or create issue.

### Contribution

just add svg icons in ./icons/:icons-name folder and create pull request agains ```develop``` after merge I will generate React components because this process is not fully automated yet.

### svg ?
svg is [supported](http://caniuse.com/#search=svg) by all major browser

### why es6 import and not fonts?

Because using ```react-icons``` you can only send icons to the users that are needed not one big font file, and also you can using this method easly figure out which icons are used in you project.

### Licence

MIT

* icons are taken from the other projects so you should check each project licence
