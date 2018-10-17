# Awk

> A versatile programming language for working on files.

- variable
`No need to declare the variable before using`

`{{$0}} - entire input record.`
`{{NF}} - number of fields in the current record.`
`{{NR}} - number of the current record.`
`{{FILENAME}} - current file name.`
`{{FS}} - (input) field separator and its default value is {{space}}`
`{{FNR}} - similar to {{NR}} but relative to the current file`
`{{OFS}} - output field separator and its default value is {{space}}.`
`{{ORS}} - output record separator and its default value is {{newline}}`

- extract the substring
`substr({{field}}, {{start}}, {{len}})`

- format the string
`printf "%s,%s,%s,%s\n", $7, $8, $9, $10`

- branch statement
`if ({{condition}}) {{body}}`

- extract certain fields within time range
`gawk -F ',' '{time=substr($5, 0, 10);if (time >= "2018-09-01" && time <= "2018-09-30") printf "%s,%s,%s,%s\n", $7, $8, $9, $10}' all.csv > slice.csv`
`input is comma separated csv, {{5th}} column is time in format {{2018-07-03 00:02:33.581103}}, output is csv with column {{7 - 10}}`

