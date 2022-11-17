# aws_lambda_nodejs



To create or update an item:Header anchor link

#Replace URL with the Invoke URL above
export INVOKE_URL="https://**abcdef123**.execute-api.eu-west-1.amazonaws.com"


Create or update an item. The command includes a request body with the item's ID, price, and name.
curl -X "PUT" -H "Content-Type: application/json" -d "{
    \"id\": \"abcdef234\",
    \"price\": 12345,
    \"name\": \"myitem\"
}" $INVOKE_URL/items

To get all items:
curl -s $INVOKE_URL/items | js-beautify 

To get an item:
curl -s $INVOKE_URL/items/abcdef234 | js-beautify

To delete an item:Header anchor link
curl -X "DELETE" $INVOKE_URL/items/abcdef234

curl -X "DELETE" $INVOKE_URL/items/abcdef234

