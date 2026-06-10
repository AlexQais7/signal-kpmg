# Signal — AI Builder Candidate Evaluation System

Built as part of the KPMG AI Builder case study submission by Alex Kais, June 2026.

## What it does
Signal evaluates whether a candidate response to an AI Builder interview question contains genuine experience signal or polished AI-generated content. It assesses authenticity and depth of real experience across five dimensions, not surface quality.

## The problem it solves
When every candidate uses AI to generate submissions, output quality converges. Traditional competency evaluators reward polished output. Signal evaluates specificity depth, tradeoff authenticity, failure texture, constraint proactivity, and problem interrogation — the signal types AI cannot fake consistently.

## Architecture
Two stage prompt pipeline using Claude Sonnet. Stage 1 extracts an evidence map from the response. Stage 2 scores each dimension citing only what was found in Stage 1. This separation prevents fabricated evidence in single pass scoring.

## To run
Open index.html in a browser. Enter your Anthropic API key when prompted.

## Built with
Claude Code, Anthropic API, vanilla HTML/CSS/JS, no dependencies.
