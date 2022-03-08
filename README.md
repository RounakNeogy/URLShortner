# sURL
## Introduction
It is a URL Shortner build with **Java** using **Objected Oriented Programming Practices** and unit tested using **JUnit**.
## Tasks' complete
- Created a short url library with required methods.
- Implemented register method to take a long URL and return a shorter URL.
- Implemented a method to lookup the long URL by providing the short URL.
- Implemented hit count to track number of long URL lookups.
- Tested this implementation with test cases.

## sUrl Interface
```Java
public interface XUrl {

  // If longUrl already has a corresponding shortUrl, return that shortUrl
  // If longUrl is new, create a new shortUrl for the longUrl and return it
  String registerNewUrl(String longUrl);

  // If shortUrl is already present, return null
  // Else, register the specified shortUrl for the given longUrl
  // Note: You don't need to validate if longUrl is already present, 
  //       assume it is always new i.e. it hasn't been seen before 
  String registerNewUrl(String longUrl, String shortUrl);

  // If shortUrl doesn't have a corresponding longUrl, return null
  // Else, return the corresponding longUrl
  String getUrl(String shortUrl);

  // Return the number of times the longUrl has been looked up using getUrl()
  Integer getHitCount(String longUrl);

  // Delete the mapping between this longUrl and its corresponding shortUrl
  // Do not zero the Hit Count for this longUrl
  String delete(String longUrl);

}
```
## Tech Stack



