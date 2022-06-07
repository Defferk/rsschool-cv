![My avatar](https://github.com/Defferk/git-lern/raw/main/1SmallLogoBW-8.png "My avatar")

### Andrey Dobretsov

### Mu contact:

- **Email** <poctadlatehnikuma@gmail.com>
- **Diskord** Defferk#0314

### About Myself:

I am 21 years old and I am a former system administrator.<br>
With the outbreak of the war, I realized that I could no longer work at the old place, and here I am, improving my skills. 

In this course I want to learn the standards of web development and decide on the direction of the future profession.

### Skills:

- HTML5, CSS3
- SQL, PHP
- C# Basics
- Adobe Photoshop, Illustrator(*But right now I'm using Serif Affinity Designer*), InDesign, Figma
- Premiere Pro, DaVinci Resolve

### My code:

```C#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;
using UnityEngine.UI;

public class RegistrationDB : MonoBehaviour{
    public InputField loginField;
    public InputField passwordField;
    public Button submitButon;
    public string url = "http://localhost/arusers/bdconect.php";
    public void CallRegister(){
        StartCoroutine(Register());
    }

    IEnumerator Register(){
        WWWForm form = new WWWForm();
        form.AddField("login", loginField.text);
        form.AddField("password", passwordField.text);
        WWW www = new WWW(url, form);        
        yield return www;
        if (www.text == "0"){
                Debug.Log("Успешное создание пользолвателя");
            }
        else{
                Debug.Log("Ошибка № " + www.text);           
            }
    }
}
```

### Work:

I worked for 2 years and over the years I managed to try many industries. <br>
I administered servers, created websites, did design work, and also repaired equipment.

### Education:

- SPBLIT (technician programmer)

- htmlacademy

### Languages:

- English \- range of A1 beginner to A2 elementary