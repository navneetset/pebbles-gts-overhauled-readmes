# Pokemon Listing Configuration

Configure the market listings for pokemon trades. This configuration allows customization of listing behavior, prices, and other aspects of pokemon trading.

## Configuration Options

- `listingMinutes`: Duration (in minutes) that a listing will remain active. Default is 2880 minutes.
- `minPrice`: Minimum price that can be set for a listing.
- `maxPrice`: Maximum price that can be set for a listing.
- `maxListings`: Maximum number of Pokemon listings a user can have at one time.
- `listingFee`: Flat fee for creating a listing. (0 for no fee)
- `listingFeePercentage`: Percentage of the listing price taken as a fee. (0.0 for no fee)

## Example Configuration

```json
{
    "listing": {
        "listingMinutes": 2880,
        "minPrice": 300,
        "maxPrice": 1000000000,
        "maxListings": 3,
        "listingFee": 0,
        "listingFeePercentage": 0.0
    }
}
```