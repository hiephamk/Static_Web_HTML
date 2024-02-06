## Tran Huynh An Duy - Table: News, 

CREATE TABLE `news` (
  `id` int NOT NULL,
  `title` varchar(50) NOT NULL,
  `news_desc` varchar(200) NOT NULL,
  `image` varchar(50) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL,
  `news_categoryId` int NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;

--
-- Dumping data for table `news`
--

INSERT INTO `news` (`id`, `title`, `news_desc`, `image`, `news_categoryId`) VALUES
(2, 'News-1', 'News about traveling today', '../andy_tasks/images/news1.jpg', 1),
(3, 'News-2', 'News about business today', '../andy_tasks/images/news2.jpg', 2),
(4, 'News-2', 'News about Technology today', '../andy_tasks/images/news3.jpg', 3);

---------


CREATE TABLE `NewsCategory` (
  `news_catergoryId` int NOT NULL,
  `catergory_name` varchar(50) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;

--
-- Dumping data for table `NewsCategory`
--

INSERT INTO `NewsCategory` (`news_catergoryId`, `catergory_name`) VALUES
(1, 'Travel'),
(2, 'Business'),
(3, 'Technologies');
