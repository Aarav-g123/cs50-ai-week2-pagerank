# AI PageRank Web Page Ranking Project

This project implements an AI-based algorithm to rank web pages by importance using the PageRank algorithm. PageRank is a method that assigns a rank to web pages based on the idea that pages with more incoming links are more important. This project provides a Python implementation of the PageRank algorithm and allows you to rank web pages within different datasets.

## Background

When search engines like Google display search results, they prioritize more "important" and high-quality pages over less important ones. One approach to determining page importance is to consider the number of incoming links a page has, as pages with more incoming links are often perceived as higher quality. The PageRank algorithm utilizes this concept to rank web pages.

## Random Surfer Model

PageRank can be conceptualized using the random surfer model. In this model, we imagine a hypothetical surfer who randomly clicks on links while navigating the internet. The PageRank of a page is interpreted as the probability that this random surfer ends up on that page.

## Iterative Algorithm

PageRank can also be defined using a recursive mathematical expression. Let PR(p) represent the PageRank of a page p, which is the probability that a random surfer lands on that page. PageRank is calculated using the following conditions:

1. With probability `1 - d`, the surfer chooses a page at random and ends up on page p. This probability is divided by the total number of pages N.
2. With probability `d`, the surfer follows a link from a page i to page p. For each page i that links to page p, the probability is proportional to `PR(i) / NumLinks(i)`, where `NumLinks(i)` is the number of links on page i.

## Usage

To run the PageRank algorithm on a specific dataset, follow these steps:

1. Clone this repository: `git clone https://github.com/Aarav-g123/PageRank-Web-Page-Ranking.git`
2. Navigate to the project directory: `cd PageRank-Web-Page-Ranking`
3. Run the PageRank algorithm on a specific dataset (e.g., corpus0):
   ```
   python pagerank.py corpus0
   ```
   Replace `corpus0` with either `corpus1` or `corpus2` as needed.

## License

This project is licensed under the MIT License. For details, please refer to the [LICENSE](LICENSE) file.

## Acknowledgments

This project was developed as part of the CS50 Introduction to Artificial Intelligence course.

## Contact

For any questions or inquiries, please contact me.
