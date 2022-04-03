# CV#1. Markdown & Git
* *1. Victor Kalevich*
* *2. [GitHub](https://github.com/AlmazerX)
  +[VK](https://vk.com/zipermax)*
* *3. Practice in the field of front-end, my main goal is to find a promising job, I took courses from myitschool, and now I am taking courses in itransition*
* **Visual Studio Code**
  + **HTML, CSS, SASS, GIT, NODE, BOOTSTRAP, AJAX, JS, JQuery, React, Figma, Photoshop**
***
### *4. Code example*
```
import React, {useEffect, useMemo, useState} from 'react'

import styles from './AppGames.module.css'

const Checkit = ({wordIndex, setWordIndex, playWords, errorWords, setErrorWords, correctWords, setCorrectWords, speak}) => {

    const randomWords = useMemo(() => playWords.sort(() => Math.random(), []))
    
    const [currentWords, setCurrentWords] = useState(['random', 'correct', 'random2'])
    
    useEffect(() => {
        setCurrentWords([
            randomWords[wordIndex].word,
            randomWords[(wordIndex + 1)%randomWords.length].word,
            randomWords[(wordIndex + 2)%randomWords.length].word,
        ].sort(() => Math.random() - 0.5))
    }, [correctWords])
    
    
    const checkWord = (word) => {
        if(word === randomWords[wordIndex].word) {
            speak(randomWords[wordIndex].translate)
            setCorrectWords(correctWords + 1)
            if(wordIndex !== playWords.length - 1) {
                setWordIndex(wordIndex + 1)
            } else {
                alert('Game is over')
            }

        } else {
            setErrorWords(errorWords + 1)
        }
    }

    return (
        <section>
            <span>Write a translation for this word</span>
            <h3>{randomWords[wordIndex].translate}</h3>
            <ul className={styles.btnContainer}>
                {currentWords.map((word, index) => (
                    <li key={index} onClick={() => checkWord(word)} className={styles.btnCheck}>{word}</li>
                ))}
            </ul>
        </section>
    )
}
export default Checkit
```
* **6. Experience in developing an application for learning English, a women's clothing store and also an online wallet**
* **7. MyItSchool, Itransition**
* **8. My English level is B2**
