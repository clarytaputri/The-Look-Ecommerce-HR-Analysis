--Import Data Employees
CREATE TABLE public.employees
(
	First_Name varchar,
	Last_Name varchar,
	Gender varchar,
	Age numeric,
	Length_Service numeric,
	Absent_Hours numeric,
	distribution_centers_id integer
);

SELECT * FROM employees

SELECT ROUND(Age,0) as Age
FROM employees;

--Import Data Age
CREATE TABLE public.Age
(
	Age numeric
);

SELECT * FROM Age

--Import Data Distribution Centers
CREATE TABLE public.distribution_centers
(
	id integer,
	name varchar,
	latitude numeric,
	longitude numeric
);

SELECT * FROM distribution_centers

--Left Join Employees with DC
SELECT
	e.First_Name,
	e.Last_Name,
	e.Gender,
	e.Age,
	e.Length_Service,
	e.Absent_Hours,
	e.distribution_centers_id,
	dc.name,
	dc.latitude,
	dc.longitude
FROM
	public.employees as e
LEFT JOIN
	public.distribution_centers as dc
ON
	e.distribution_centers_id = dc.id