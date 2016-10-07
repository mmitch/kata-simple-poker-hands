# Simple Poker Hands programming kata

This kata is based on the
[Poker Hands Kata](http://codingdojo.org/cgi-bin/index.pl?KataPokerHands),
but it is much simpler. I’ve come across this version multiple times
but I could not find it anywhere on the web yet, so I’ll share it
here:

## Goal of the kata

You shall write a simple algorithm to parse a poker hand (a deck
consisting of some cards) and report the highest card combination from
the hand.

## Card representations

A card is represented as a simple string like ``H10`` for the Ten of
Hearts or ``SA`` for the ace of Spades.

A hand is represented as a space-separated string of cards:
``C5 S1 H5 CK HQ``

The card ranks are:

* numbers ``2`` to ``10``
* ``J`` Jack
* ``Q`` Queen
* ``K`` King
* ``A`` Ace

The card suits are:

* ``S`` Spades
* ``H`` Hearts
* ``D`` Diamonds
* ``C`` Clubs

## Scoring

To make this simple, you should only care about single cards (High
Card) and Pairs, where any pair is higher than any single card.

Cards ranks are ordered as shown above (``2`` is lowest, ``A`` is
highest).

Card suits are not relevant for scoring.

## Examples

* given input ``D8 H3 S9 CJ D2`` => expected output ``CJ``
* given input ``S3 D5 CJ D3 S7`` => expected output ``S3 D3``
