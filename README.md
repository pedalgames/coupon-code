# Coupon Code Generator

This is a flexible coupon code generator.

## Static Usage

```php
\Ryantxr\CouponCode\Generator::generate(); // generate a code
\Ryantxr\CouponCode\Generator::generate(true); // generate a lowercase code
\Ryantxr\CouponCode\Generator::generate(true, $bytes); // generate a lower case code and pass in the random bytes
\Ryantxr\CouponCode\Generator::init(['numberOfSegments' => 5, 'segmentLength' => 4])->generateCode(); // generate a code
```

## Use as an object

```php
$codeGenerator = new \Ryantxr\CouponCode\Generator();
$codeGenerator = new \Ryantxr\CouponCode\Generator(['numberOfSegments' => 5, 'segmentLength' => 4]);

$code = $codeGenerator->generate();
$code = $codeGenerator->generate(true); // generate a lowercase code
$code = $codeGenerator->generate(true, $randomBytes); // generate a lowercase code, passing in the random bytes
```

## See also

[perl](https://github.com/grantm/Algorithm-CouponCode)

[NodeJS](https://www.npmjs.com/package/coupon-code)

[Ruby](https://rubygems.org/gems/coupon_code/versions/0.0.1)

[php](https://github.com/atelierdisko/coupon_code)


    - git add . && git commit -m'initial'
