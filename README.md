db: graphql-sample



use graphql-sample

db.createUser(
{
     user: "graphQLUser",
     pwd: "graphQLUser",
     roles: [
        { role: "userAdmin", db: "graphql-sample" }
     ]
   }
)

mongo "mongodb://graphQLUser:graphQLUser@127.0.0.1:27017/graphql-sample"

collection(s):
