# atom-angular-snippets
A collection of Angular JS snippets for Atom, following [Todd Motto's styleguide](https://github.com/toddmotto/angularjs-styleguide).

To use, just copy and paste your snippet of choice into your snippets.cson file in atom:

    Edit > Open Your Snippets

Angular Module

`ng-mod[tab]` produces:

	(function(){
	
		'use strict';
	
		angular
			.module('app');
	
	})();

`ng-ctrl[tab]` produces:

	(function(){

		'use strict';

		angular
			.module('app')
			.controller('AppController', AppController);

			AppController.$inject = [];

			function AppController(){

				var vm = this;

			}

	})();

`ng-fil[tab]` produces:

	(function(){

		'use strict';

		angular
			.module('app')
			.filter('myFilter', myFilter);

			function myFilter(){

				return items.filter(function(item) {
	                		return item;
	                        });
	                        
			}
			
	})();

`ng-dir[tab]` produces:

    (function(){

        'use strict';

        angular
            .module('app')
            .directive('myDirective', myDirective);

        myDirective.$inject = [];

        function $1() {
                    return {
                        restrict: '',
                        templateUrl: '',
                        scope: {},
                        controller: function($scope, $element, $attrs){

                        }
                    }
                }

    })();
