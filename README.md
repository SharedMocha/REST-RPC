RPC- Used to make procedure calls between process. WHwich means we can directly call js functions which makes life much easier.
It always has one url and can talk on multiple protocals .WHich means more than HTTP
We use protocal buffer for serializng structed data for transmittion between process/systems.
Uses get,post

REST- Works only on http
Uses nouns as colelctions
http://18.216.147.18:4000/channels/common/transactions/bf014e5635b4dd38225dc54d592ed1b1403fd9ace2f5d90ac512fbbc11b133aa?peer=peer1
get transaction bf0... from transactions colleciton
Uses http put,get.delte,post
200-good
400-client error
500-server error

Any design tlaks about cahcing,pagination,sorting
cacahing can be done both at client level and also server level.
CLient level using cahcing paramters in headers like expire
server side by storing data on file so we can send it againa and again to client rather than making a new clal to db
**Remeber restis stateless** which means server will not store anything-Its an advantage as we can query and get reuslts easily
or use inmeneory achcing softwares for faster performace


pagination -can be doen in 2 ways-app layer/db layer
db layer is using limit and offset in mysql select clause
or
passing keyvalue such as data param to query to so we can get next batch of results

sorting-
send sort clause in rest api and db does the heavy lifting or app layer using data structures
https://www.moesif.com/blog/technical/api-design/REST-API-Design-Filtering-Sorting-and-Pagination/

http://www.drdobbs.com/web-development/restful-web-services-a-tutorial/240169069
