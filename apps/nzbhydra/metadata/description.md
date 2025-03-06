# NZBHydra 2 is a meta search for newznab indexers and torznab trackers

NZBHydra 2 is a meta search for newznab indexers and torznab trackers. It provides easy access to newznab indexers and many torznab trackers via Jackett. You can search all your indexers and trackers from one place and use it as an indexer source for tools like Sonarr, Radarr, Lidarr or CouchPotato.
Major Features

    Searches Anizb, BinSearch, NZBIndex and any newznab compatible indexers. Merges all results, filters them by a number of configurable restrictions, recognizes duplicates and returns them all in one place
    Add results to NZBGet or SABnzbd
    Support for all relevant media IDs (IMDB, TMDB, TVDB, TVRage, TVMaze) and conversion between them
    Query generation, meaning a query will be generated if only a media ID is provided in the search and the indexer doesn't support the ID or if no results were found
    Compatible with Sonarr, Radarr, NZBGet, SABnzbd, nzb360, CouchPotato, Mylar, LL, Sick Beard, Jackett/Cardigann, Watcher, etc.
    Search and download history and extensive stats. E.g. indexer response times, download shares, NZB age, etc.
    Authentication and multi-user support
    Automatic update of NZB download status by querying configured downloaders
    RSS support with configurable cache times
    Torrent support:
        For GUI searches, allowing you to download torrents to a blackhole folder
        A separate Torznab compatible endpoint for API requests, allowing you to merge multiple trackers
    Extensive configurability
    Save torrents in a black hole folder; Torznab API endpoint
    Migration of database and settings from v1


If you want to know more you can head over to our website: [https://github.com/theotherp/nzbhydra2/](https://github.com/theotherp/nzbhydra2/).

## Folder Info

| Root Folder                           | Container Folder |
|---------------------------------------|------------------|
| /runtipi/app-data/nzbhydra/config | /config          |
| /runtipi/media/usenet                 | /media/usenet    |