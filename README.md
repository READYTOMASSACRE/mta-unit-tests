# mta-unit-tests
Simply lib for testing mta scripts
Docs about lunity lib: 
https://github.com/Phrogz/Lunity
-- Example test
-- @usage
-- First, we need unit test in global table
-- Then, we can describe tests

g_Tests[#g_Tests+1] = {
  -- Description of testSuite
  ["_NAME"] = "testSuite:example simplify assert test, should return true",
  -- Name of assert
  ["testExample"] = function()
    assert(true, "that was true!")
  end,
  -- Second name another assert
  ["testAnotherExample"] = function()
    assertEqual(true, false, "that second assert, should equals!")
  end
}
