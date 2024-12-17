<!--hide-->
# Urban Dictionary Terminal App
<!--endhide-->

![Urban Dictionary Terminal App](https://github.com/breatheco-de/english-dictionary-project-tutorial/blob/master/preview.gif?raw=true)

The [Urban Dictionary](https://www.urbandictionary.com/) is an amazing resource for english language lovers; It features accurate definitions of words, not like other services like Wikipedia, Oxford, etc. 😅

In this project, you are going to build a terminal based (CLI) dictionary.

### Before you begin

1. Register a [RapidAPI.com](https://rapidapi.com/) account and make your to request a key for the [urban dictionary API](https://rapidapi.com/community/api/urban-dictionary).
2. Watch this 15 min video to [understand pipenv](https://www.youtube.com/watch?v=6Qmnh5C4Pmo), the python package manager.
3. Watch this 10 min video on [what are API Keys and credentials](https://www.youtube.com/watch?v=InoAIgBZIEA).

<onlyfor saas="false" withBanner="false">

## 🌱 How to start this project

This project includes the necessary files to get started, and you have two options to begin:

a) Open this link with [Codespaces](https://4geeks.com/lesson/what-is-github-codespaces) (recommended) or [Gitpod](https://4geeks.com/lesson/how-to-use-gitpod) in your browser: https://s.4geeks.com/start?repo=breatheco-de/urban-dictionary-project-tutorial

b) Clone this repository locally on your computer:

```sh
$ git clone https://github.com/breatheco-de/urban-dictionary-project-tutorial
```

### Steps

1. Install the application dependencies (only once):

```bash
$ pipenv install
```

2. Run the application by typing (each time):

```bash
$ pipenv run python app.py
```

💡 Important: Remember to update the project's `remote` URL to your repository using `git remote set-url origin <your new url>`, and then save your code to your new repository using `add`, `commit`, and `push`.

</onlyfor>

### 📝 Features that the application must have

1. Greet the user
2. Ask the user for the term he/she wants to look up, use the `input("What term do you want to look for?")` python function.
3. Use the python requests package to code your GET request to the Urban Dictionary API

Let's suppose that we are looking for the definition of the word `computer`
The API specification says that you have to do a GET request to the following URL: 

```python
url = "https://mashape-community-urban-dictionary.p.rapidapi.com/define?term=computer"
```

Don't forget to add the `headers` with the API credentials, please refer to [the API example in the documentation](https://rapidapi.com/community/api/urban-dictionary/endpoints).

4. Process the response body, understand it, and get the word definition from the incoming response body.
5. Show the definition on the terminal.
6. Store the definition in a JSON file.

### 🤠 Feeling confident?

The following requirements are not mandatory, but you can try completing them if you feel confident:

1. Cache system: If the user asks for the same word again, instead of calling the API again, you should have the previous responses stored in a `dict`.
2. Look for multiple words separated by comma.
3. Use `sys.argv` to allow the user to ask for a definition like this:

```python
# "enjoy" is the word the user is looking up the definition
$ pipenv run python app.py enjoy
```

Hint: [how to use the sys.argv](https://www.pythonforbeginners.com/system/python-sys-argv)



