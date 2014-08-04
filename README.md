# ca-helpers

Various helpers and utilities for AngularJS apps I regularly need.

## Services

### ca-helpers-apply

This service provides a $rootScope.apply method and service method which
takes a single *$scope* as an argument, and safely calls the apply() method on
the scope, taking account of all the conditions where it could potentially
cause issues.

Useful for getting around issues where you have some kind of async that isn't
built in with Angular's event mechanisms.