cmake_minimum_required(VERSION 3.5)
project(boost-lexical_cast)

add_library(boost_lexical_cast INTERFACE)
add_library(Boost::lexical_cast ALIAS boost_lexical_cast)

target_include_directories(boost_lexical_cast INTERFACE include)

target_link_libraries(boost_lexical_cast
	INTERFACE
		Boost::array
		Boost::assert
		Boost::config
		Boost::container
		Boost::core
		Boost::integer
		Boost::math
		Boost::mpl
		Boost::numeric_conversion
		Boost::range
		Boost::static_assert
		Boost::throw_exception
		Boost::type_traits
)