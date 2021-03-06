<a href="https://codeclimate.com/github/davidesantangelo/feedi/maintainability"><img src="https://api.codeclimate.com/v1/badges/e84db3d81a5e9935d63a/maintainability" /></a> <img src="https://img.shields.io/github/tag/davidesantangelo/feedi.svg"/> <a href="https://github.com/eonu/arx/blob/master/LICENSE"><img src="https://camo.githubusercontent.com/ad562cdf422b103f1a409db66ba31cb79414594d/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f656f6e752f6172782e737667" alt="License" data-canonical-src="https://img.shields.io/github/license/eonu/arx.svg" style="max-width:100%;"></a> [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/davidesantangelo/feedi/issues) [![Open Source Helpers](https://www.codetriage.com/davidesantangelo/feedi/badges/users.svg)](https://www.codetriage.com/davidesantangelo/feedi)
 <img src="https://img.shields.io/github/languages/top/davidesantangelo/feedi.svg"/>

# FeediRSS
*The best RESTful RSS experience you can find.*

FeediRSS turns feed data into an awesome API. The API simplifies how you handle RSS, Atom, or JSON feeds. You can add and keep track of your favourite feed data with a simple, fast and clean REST API. All entries are enriched by Machine Learning and Semantic engines.

## Search Engine

Take a look at a little search engine developed in React around this API. 

www.datorss.com

Feedback is welcome on [its repository](https://github.com/davidesantangelo/datorss).


## Example

``` bash

curl 'https://api.feedirss.com/search/entries?q=news' | json_pp

{
  "data": [
    {
      "id": "86b0f829-e300-4eef-82e1-82f34d03aff6",
      "type": "entry",
      "attributes": {
        "title": "\"Pandemic, Infodemic\": 2 Cartoon Characters Battling Fake News In Assam",
        "url": "https://www.ndtv.com/india-news/coronavirus-pandemic-infodemic-2-cartoon-characters-battling-fake-news-in-assam-2222333",
        "published_at": 1588448805,
        "body": "An English daily in Assam's Guwahati has been publishing a cartoon strip to tackle the fake news related to the coronavirus pandemic. The two central characters- \"Pandemic and Infodemic\"- are being...<img src=\"http://feeds.feedburner.com/~r/NDTV-LatestNews/~4/lEmH201Q8jI\" height=\"1\" width=\"1\" alt=\"\"/>",
        "text": "An English daily in Assam's Guwahati has been publishing a cartoon strip to tackle the fake news related to the coronavirus pandemic. The two central characters- \"Pandemic and Infodemic\"- are being...",
        "categories": [
          "all india"
        ],
        "sentiment": null,
        "parent": {
          "id": "c97bdae6-b5d1-4966-b9f3-615e29d4d47d",
          "title": "NDTV News  -  Special",
          "url": "feed:http://feeds.feedburner.com/NDTV-LatestNews",
          "rank": 99
        },
        "tags": []
      },
      "relationships": {
        "feed": {
          "data": {
            "id": "c97bdae6-b5d1-4966-b9f3-615e29d4d47d",
            "type": "feed"
          }
        }
      }
    },
  ]
}

```
## Wiki

All documentation is in the Wiki section. Feel free to make it better, of course.

https://github.com/davidesantangelo/feedirss-api/wiki

## Built With

- [Ruby on Rails](https://github.com/rails/rails) &mdash; Our back end API is a Rails app. It responds to requests RESTfully in JSON.
- [PostgreSQL](https://www.postgresql.org/) &mdash; Our main data store is in Postgres.
- [Redis](https://redis.io/) &mdash; We use Redis as a cache and for transient data.
- [Feedjira](https://github.com/feedjira/feedjira) Feedjira is a Ruby library designed to parse feeds.
- [ElasticSearch](https://www.elastic.co/products/elasticsearch) Elasticsearch is a distributed, RESTful search and analytics engine.
- [Dandelion](https://dandelion.eu) Semantic Text Analytics as a service.
- [Sidekiq](http://sidekiq.org) Simple, efficient background processing for Ruby.
- [FastJSONAPI](https://github.com/Netflix/fast_jsonapi) A lightning fast JSON:API serializer for Ruby Objects.
- [Searchkick](https://github.com/ankane/searchkick) Intelligent search made easy.

Plus *lots* of Ruby Gems, a complete list of which is at [/master/Gemfile](https://github.com/davidesantangelo/feedi/blob/master/Gemfile).

## Buy me a coffee

If you want to support me in server costs to keep FeediRSS free and up, consider buying me a coffee! Thanks!

<a href="https://www.buymeacoffee.com/582rhJH" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>


## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/davidesantangelo/feedirss-api. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
