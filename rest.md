# REST

## @Controller and @RestController

- As you can see in Spring documentation (_Spring RestController Documentation_) Rest Controller annotation is the same as Controller 
annotation, but assuming that `@ResponseBody` is active by default, so all the json are parsed to java objects. 
- If you use `@Controller` you can return a view in Spring webMVC.
