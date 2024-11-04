- 👋 Hi, I’m @kioNinjae
Generating 3, 4, 5, and 6 Digit OTP Payloads for Brute-Force and Rate Limit Testing

To evaluate application security against brute-force attacks, you can generate OTP combinations using the following commands:

Command to Generate OTPs:
For 3 Digits:

echo -e {000..999} | sed 's/ /\n/g' >> output_filename.txt
For 4 Digits:


echo -e {0000..9999} | sed 's/ /\n/g' >> output_filename.txt
For 5 Digits:


echo -e {00000..99999} | sed 's/ /\n/g' >> output_filename.txt
For 6 Digits:

echo -e {000000..999999} | sed 's/ /\n/g' >> output_filename.txt
Explanation:
echo -e: Generates a sequence of numbers.
sed 's/ /\n/g': Converts spaces to newlines, placing each OTP on a separate line.
>> output_filename.txt: Appends the output to a specified file.
