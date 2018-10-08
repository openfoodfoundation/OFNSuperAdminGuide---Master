# Translate in your own language

### How we organize translations in OFN

Before you can start translating the OFN, you need to be added to [Transifex](https://www.transifex.com/open-food-foundation/open-food-network/) which is the tool we use to do distributed translation work. There is a separate translation file per language AND per territory, for instance there is French-France and French-Canada. This is not only because languages gave variants locally, but also because some of the things translated concerns directly business related information, like business model, and you won't just translate but also update information to your local business model.

It's important to understand how Transifex works: whenever a new feature or line of text is added to OFN, it will create a new "entry" in Transifex that as a language translator you will have to translate. When you have translated to 100% your language localization file is "pushed" to the master OFN code so when you upgrade the code in your local server, you will have the new translation. If you don't translate to 100% developers need to manually "pull" your translation to include them in the code.

So the good practice we recommend is : when a new release is about to be made, developers will ask translators to go into Transifex and translate everything, so that when the release happen things have been translated.

### Single language translation

#### Some strings that you need to be careful about

* For the key **"language\_name"** be careful, the source string is "English" but you have to translate to your own language name, like "Deutch", "Français", "Italiano", etc. This string displays in the dropdown multilingual menu on all OFN pages

![](.gitbook/assets/multilingual.png)

* For the key **"menu\_"** those keys represent the menu titles and redirection pages when you clic on this menu. For some menu they will redirect to internal pages, like "shops", so the link will be "/shops". But others like "about" will redirect to external pages, like a wordpress website, so in that case you can put your url in the adequate translation entry.

![](.gitbook/assets/capture-du-2018-10-08-10-42-48.png)

### Multi-lingual instance

Some information types can only be in one language e.g. Product Categories don't get translated





