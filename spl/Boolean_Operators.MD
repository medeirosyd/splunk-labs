# Boolean operators

The Splunk search processing language (SPL) supports the following logical operators in Boolean expressions: AND, OR, NOT, and XOR.

## Sample usage

host="www1" AND status=200 OR action="addtocart"

host="www1" AND (status=200 OR action="addtocart")

host="www1" NOT status=200

host="www1" NOT status=200 AND NOT status=505

host="www1" NOT (status=200 OR status=505)
