Node wrapper for the [We the People API](https://petitions.whitehouse.gov/developers)
================

node-wethepeople provides a node wrapper for the White House's [We the People API](https://petitions.whitehouse.gov/developers).

The wrapper is only configured to provide JSON responses.

# API Methods

The schemas defining the objects accepted by these methods can be found in [lib/api_schema.js](https://github.com/l12s/node-wethepeople/blob/master/lib/api_schema.js)

## [Petitions](https://github.com/l12s/node-wethepeople/blob/master/lib/petitions.js)

- **<code>GET</code> getPetition** - fetches a single petition
- **<code>GET</code> searchPetitions** - fetches petitions matching the supplied query object
- **<code>GET</code> getSignatures** - fetches signatures on a specific petition matching the supplied query object

## [Signatures](https://github.com/l12s/node-wethepeople/blob/master/lib/signatures.js)

- **<code>POST</code> signPetition** - signs a petition via the API, causing a validation email to be sent to the supplied email address by the WtP API to confirm signature

## [Validations](https://github.com/l12s/node-wethepeople/blob/master/lib/validations.js)

- **<code>GET</code> getValidations** - gets the validations associated with the supplied petition
