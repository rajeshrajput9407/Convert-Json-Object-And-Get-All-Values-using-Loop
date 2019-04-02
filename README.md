# Convert-Json-Object-And-Get-All-Values-using-Loop
Convert Json Object And Get All Values using Loop
```

string source = "{\r\n   \"id\": \"100000280905615\", \r\n \"name\": \"Jerard Jones\",  \r\n   \"first_name\": \"Jerard\", \r\n   \"last_name\": \"Jones\", \r\n   \"link\": \"https://www.facebook.com/Jerard.Jones\", \r\n   \"username\": \"Jerard.Jones\", \r\n   \"gender\": \"female\", \r\n   \"locale\": \"en_US\"\r\n}";
           

            dynamic jsonObj = JsonConvert.DeserializeObject(source);

            foreach (var obj in jsonObj)
            {
                string ss = obj.ToString();
                string[] fdf = ss.Split(':');
                string dd = fdf[1];
                //Console.WriteLine(obj.address);
                string sss = dd.Replace("\"", "").Trim();
                
                ```
