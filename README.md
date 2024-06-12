--this is very simple crud with user data issue, 

-- phpMyAdmin SQL Dump
-- version 5.2.1
-- https://www.phpmyadmin.net/
--
-- Host: 127.0.0.1
-- Generation Time: Jun 12, 2024 at 08:18 AM
-- Server version: 10.4.28-MariaDB
-- PHP Version: 8.2.4

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Database: `codeigniter`
--

-- --------------------------------------------------------

--
-- Table structure for table `tbl_user`
--

CREATE TABLE `tbl_user` (
  `user_no` int(11) NOT NULL,
  `user_name` varchar(125) DEFAULT NULL,
  `user_email` varchar(125) DEFAULT NULL,
  `user_password` text DEFAULT NULL,
  `user_photo` text DEFAULT NULL,
  `user_akses` varchar(50) DEFAULT NULL,
  `user_detail` text DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `tbl_user`
--

INSERT INTO `tbl_user` (`user_no`, `user_name`, `user_email`, `user_password`, `user_photo`, `user_akses`, `user_detail`) VALUES
(1, 'Irfan', 'irfan_chibenk25@gmail.com', '', 'user_20240611075445.gif', 'Admin', ' Kawaii'),
(2, 'Administrator', 'admin@local', 'admin', 'user_20240611070827.gif', 'Admin', '  Administrator'),
(4, 'Muhammad Akhdan AlMaliki', 'akhdan@local', '123', 'default.jpg', 'User', '    Muhammad Akhdan AlMaliki'),
(8, 'Code Igniter 4', 'ci4@local', 'ci4', 'donuts4_2.gif', 'Admin', ' Code Igniter 4');

--
-- Indexes for dumped tables
--

--
-- Indexes for table `tbl_user`
--
ALTER TABLE `tbl_user`
  ADD PRIMARY KEY (`user_no`);

--
-- AUTO_INCREMENT for dumped tables
--

--
-- AUTO_INCREMENT for table `tbl_user`
--
ALTER TABLE `tbl_user`
  MODIFY `user_no` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=9;
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
