# Auth API - Service #

## Abstract ##
Auth Service is a centralized product to manage user credentials for all products provided by Quantico

## Terminology ##
--

## Context ##
Each application has users, and they need simple or complex authentication and validation to get into the app. 
Quantico is planning to centralize authentication for all users with some security rules and mechanism specialized to these credentials

## Goals ##
[User Stories](/user_stories/list.md ':include')

## Out of Scope ##
For now  we only provide the endpoints and logic to manage authentication. Do not have frontend to manage credentials by itself

## Future Goals ##
Include some frontend integration and provide access like Google Auth of Facebook Auth

## Current Solution ##
Before this launch, the credentials were spread and using different logic on each product.

## Proposed Solution ##
Centralized the authentication managing
