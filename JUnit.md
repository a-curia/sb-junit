JUnit
-----

 

**\@BeforeClass**

-   Run once before any of the test methods in the class, public static void

-   Run once, e.g. Database connection, connection pool

**\@AfterClass**

-   Run once after all the tests in the class have been run, public static void

-   Run once, e.g close connection, cleanup

**\@Before**

-   Run before \@Test, public void

-   e.g. Creating an similar object and share for all \@Test

**\@After**

-   Run after \@Test, public void

**\@Test**

-   This is the test method to run, public void
