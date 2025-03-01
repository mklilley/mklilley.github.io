# mattlilley.com

Source code for mattlilley.com

## About the website code

This website is built using [Hugo](https://gohugo.io/) (version 0.144.2) - it's a static website generator that takes simple markdown files and turns them into webpages. It does this by through the use of templates written in the [Go](https://go.dev/) language. 

What's great about Hugo is that we don't have to create these templates from scratch - there are many [themes](https://themes.gohugo.io/) that we can use out of the box.

## Editing the website code

### Cloud
Every time you edit a file on the `main` branch here on Github, an [Action](/.github/workflows/hugo.yml) runs behind the scenes to compile the website and deploy it to Github's servers which will point to [mattlilley.com](https://mattlilley.com).

This approach is good for doing a small number of edits. If you're doing a lot of editing then it's better to work locally where you can edit and see the results of your changes in real time.

### Local
Hugo allows you to run what's called a local "dev server" which let's you to make edits locally and see the results in real time. In order to do this you need to install a couple of things:
- [Go](https://go.dev/dl/)
- [Hugo](https://gohugo.io/installation/)

For installing Hugo on **Mac**, the simplest way is running 

```
brew install hugo
```

For installing Hugo on **Windows** the simplest way is running 

```
choco install hugo-extended
```


After installing, go ahead and clone the repo

```
git clone https://github.com/mklilley/mklilley.github.io
```

And then go into the directory and run this to get your dev server started.

```
hugo server -D
```

> Note, the `-D` will render content that is marked as "Draft". If you're curious to see what Hugo is actually generating, then check out the `public` folder.
