# An Italian corpus for content sensitivity analysis: ITA-SENS

ITA-SENS is a new dataset consisting of more than 15 000 social media posts written in Italian. In this work, we rely on the anonymity assumption, i.e., we consider as sensitive all posts that have been posted anonymously, while posts posted publicly are considered non-sensitive. Hence, we focus on Italian and identify two sources of non-anonymous and anonymous posts: Twitter and [Insegreto](https://insegreto.com/it). Regarding first source, we take into account FEEL-IT (Bianchi et al.) and SENTIPOLC (Barbieri et al.), two corpora of Italian tweets covering a wide range of generic topics. 

[FEEL-IT](https://github.com/MilaNLProc/feel-it) is a corpus of tweets written in Italian and annotated according to four base emotions: anger, fear, joy and sadness. The curators of this dataset have downloaded tweets at a daily basis, by monitoring trend topic in a three-month period. The dataset consists of 1000 tweets per day covering different topics, including health, sports, societal problems and TV programs. Topics have different time-spans, from hours (e.g., tweets related to TV programs) or days (e.g., major sports events) to the entire observation period (general topics such as COVID-19). 

[SENTIPOLC](https://github.com/evalita2016/data), instead, is a dataset consisting of tweets written in Italian and constructed to solve sentiment polarity classification. It has been presented during [EVALITA 2016](https://www.evalita.it/), a periodic evaluation campaign of Natural Language Processing (NLP) and speech tools for the Italian language. Each tweet is annotated according to its topic, however, since most of them are related to a very specific political topic, we only retain 295 tweets addressing more different and general subjects. Additionally, to broaden the variety and quantity of tweets, we downloaded further tweets directly from Twitter, by filtering them according to popular general hashtags or by downloading them from news accounts, using the official Twitter API.

As anonymous source, we take into consideration posts from [Insegreto](https://insegreto.com/it) (the Italian locution "in segreto" means "secretly" in English), an Italian social network that allows people to share their lives, secrets and opinions on different topics, in a totally anonymous way. Posts are organized into several categories ranging from school to health, from politics to religion, from love to sexuality. As such, this is a valuable source of sensitive posts.

ITA-SENS consists of 15 144 Italian posts, of which 8 419 are labeled as sensitive and 6 725 as non-sensitive. We split it randomly by putting 55\% of the data into the training set; 25\% into the validation set and the remaining 20\% into the test set.

## Annotation

Exactly as was done in previous studies (Correa et al.), for the annotation of our corpus we rely on the anonymity assumption, where the content is considered sensitive if the user has chosen to publish it anonymously, hiding their real identity or if they have made it visible to only some friends. If the content is visible to anyone or the author can be identified from it, then it is considered non-sensitive. After a careful reading and analysis of the collected posts, we have observed that, effectively those coming from Insegreto contain sensitive information that could harm the privacy of both the author and other identifiable people. Furthermore, they deal with sensitive topics and are published in a totally anonymous way. For these reasons, we label all Insegreto posts as privacy-sensitive. On the other hand, we consider all tweets in the corpus as non-sensitive because they come from public Twitter pages and profiles, following the anonymity assumption. Although it has been shown that this assumption is simplistic (Bioglio et al.), we rely on it for this work, as the main goal is to study whether multilingual text analysis approaches can compete with monolingual ones for the specific task of content sensitivity analysis.

## Citation



## License

This dataset is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. 

You are free to:
- Share — copy and redistribute the material in any medium or format
- Adapt — remix, transform, and build upon the material for any purpose, even commercially. 

The licensor cannot revoke these freedoms as long as you follow the license terms.

Under the following terms:
- Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
- ShareAlike — If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.
- No additional restrictions — You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

Notices:
- You do not have to comply with the license for elements of the material in the public domain or where your use is permitted by an applicable exception or limitation.
- No warranties are given. The license may not give you all of the permissions necessary for your intended use. For example, other rights such as publicity, privacy, or moral rights may limit how you use the material.

To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/ 
