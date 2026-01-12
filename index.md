---
layout: default
title: Ben Casselman
---

# Ben Casselman
**Chief Economics Correspondent, The New York Times**

I am an economics reporter for The New York Times, where I cover the economy, labor markets, and data-driven business stories. I am also an adjunct professor at the Craig Newmark Graduate School of Journalism at CUNY.

Previously, I was the chief economics writer for *FiveThirtyEight* and a reporter for *The Wall Street Journal*. My work often focuses on the intersection of complex statistics and human storytelling.

---

### Significant Stories
* **[Deepwater Horizon Coverage](https://www.wsj.com/...)** – Finalist for the Pulitzer Prize in National Reporting and winner of a Gerald Loeb Award.
* **[Gun Deaths in America](https://fivethirtyeight.com/features/gun-deaths/)** – An award-winning data investigation into the reality of firearm violence.
* **[The Great Resignation](https://www.nytimes.com/...)** – Defining the post-pandemic labor shift.

---

### Recent Reporting
<div id="rss-feed">Loading recent stories...</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/rss-parser/3.12.0/rss-parser.min.js"></script>
<script>
  const RSS_URL = `https://rss.nytimes.com/services/xml/rss/nyt/Economy.xml`; // Or your specific author feed if available
  const parser = new RSSParser();

  parser.parseURL('https://cors-anywhere.herokuapp.com/' + RSS_URL, function(err, feed) {
    if (err) throw err;
    let html = '<ul>';
    // Filter feed for items containing "Ben Casselman" if using a general Economy feed
    const myStories = feed.items.filter(item => item.creator === "Ben Casselman" || item.content.includes("Ben Casselman")).slice(0, 5);
    
    myStories.forEach(item => {
      html += `<li><a href="${item.link}" target="_blank"><strong>${item.title}</strong></a> - ${new Date(item.pubDate).toLocaleDateString()}</li>`;
    });
    html += '</ul>';
    document.getElementById('rss-feed').innerHTML = html;
  });
</script>

---

### Contact
The best way to reach me is via email at [ben.casselman@nytimes.com](mailto:ben.casselman@nytimes.com). 

[LinkedIn](https://www.linkedin.com/in/bencasselman/) | [NYT Bio](https://www.nytimes.com/by/ben-casselman) | [Twitter](https://twitter.com/bencasselman)
